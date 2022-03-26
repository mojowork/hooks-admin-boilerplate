# hooks-admin

### 初始化

```bash
# 使用 ts 模版
npx create-react-app hooks-admin --template typescript
```

### 添加代码格式化

```bash
# 安装 Prettier
yarn add --dev --exact prettier

# 整理配置
echo {}> .prettierrc.json
touch .prettierignore

# Ignore artifacts:
build
coverage

# Pre-commit Hook
npx mrm@2 lint-staged
```

### commitlint

```bash
yarn add @commitlint/{config-conventional,cli} -D
yarn husky install
yarn husky add .husky/commit-msg 'yarn commitlint --edit $1'
```

### 本地数据 Mock

```bash
# 全局安装
sudo npm install -g json-server
echo {}> db.json
json-server --watch db.json

```

```json
{
  "posts": [{ "id": 1, "title": "json-server", "author": "typicode" }],
  "comments": [{ "id": 1, "body": "some comment", "postId": 1 }],
  "profile": { "name": "typicode" }
}
```

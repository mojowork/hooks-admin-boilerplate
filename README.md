# hooks-admin

### 初始化

`bash

# 使用 ts 模版

npx create-react-app hooks-admin --template typescript
`

### 添加代码格式化

`bash

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
`

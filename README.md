# Introduction

本项目用于演示使用asciidoctor-maven插件以及对应的spring扩展生成spring风格的html文档以及使用GitHub Action构建CI/CI流程将文档自动发布到GitHub Pages

重点包括：
- src/main/asciidoc下存放原始的asciidoc文档
- pom.xml中配置asciidoctor-maven插件
- .github/workflows下存放GitHub Action配置
- 执行mvn clean package后target/generated-docs目录下会生成原始asciidoc文档转换后的html文件
- git push后会触发CI/CI流程执行，将修改后的页面自动部署到GitHub Pages
- 访问GitHub Pages的地址为https://pxzxj.github.io/asciidoc-cicd-demo

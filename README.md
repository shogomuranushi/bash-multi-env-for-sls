# Serverless Framework Template for bash for multiple environment

This is a template for deploying Lambda using bash/shell script with Serverless Framework.
In addition, it includes serverless.yml optimized for using multiple environments such as dev, stage and production.

## How To

### Getting Started

Get started in 3 steps

```
$ npm install serverless -g
$ serverless create --template-url https://github.com/shogomuranushi/bash-multi-env-for-sls && cd bash-multi-env-for-sls
$ serverless deploy
```

### How to change the processing content of bash script

1. Change inside of function hundler {} in function.sh

### How to process before bash script startup (pip, etc..)

1. Add before the while of bootstrap file

### How to change region for each environment

1. Modify ./conf/xxx.yml

### How to add items to change for each environment

1. Add ./conf/xxx.yml
2. Add ${self:custom.env.file.${self:provider.stage}.xxxxxx} to serverless.yml

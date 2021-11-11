# Makefile

1. Environment Variables
  1. Load environment variables from file if exists 

## Environment Variables 

### Load environment variables from file if exists

```Makefile
#!make

-include .env
export $(shell test -f .env && cut -d= -f1 .env)
```

# GO Web App

This Web app is a project built with React, Mongo and Go.

## Group Division
|  任务   | 人员  |
|  ----  | ----  |
| 前端 | 伍浩源，赵文序 |
| 后端及测试  | 谢正雄， 周景伟， 周京有 |



## Requirements and Environment

As you can see, the requirements and configure of environment is in the 'Environment setup' part of README.

Moreover, we need to build the environment of database.

## Features

- Sign in and Sign up
- Store List (Main Page)
    - Users can view the commodities in store list.
- Shopping cart
    - The commodities that users want to buy will be showed in the shopping cart.

## Database Sources

- user
    - username (string)
    - password (string)
    - remaining sum (double)

- commodity
    - name (string)
    - introduction (string)
    - picture (string - picture path )
    - price (double)

- comment
    - username (string)
    - commodity name (string)

- shopping cart
    - username (string)
    - commodity list (list[commodity, commodity, ...])

## API Test
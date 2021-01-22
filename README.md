##uesrs table

| colum      | type | option              |
|:-----------|------------:|:------------:|
| mail       | string      | null: false  |
| pass       |  string     | null: false   |
| passconf   | string      | null: false  |
| username   |  string     | null: false  |
| profile    | strings     | null: false  |
| belonging  | string      | null: false  |
| position  | string      | null: false  |
###Association
has_many :comments
has_many :prototype


prototypes table

| colum      | type        | option             |
|:-----------|------------:|:------------:      |
| name       | string      | null: false        |
| catchcopy  | string      | null: false        |
| concept    | string      | null: false        |


###Association
has_many :comments
belongs_to :user


comments table

| colum           | type        | option             |
|:-----------     |------------:|:------------:      |
| text            | string      | null: false        |

###Association
belongs_to: prototype
belongs_to: user


画像投稿はActive Storage
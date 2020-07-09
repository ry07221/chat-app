## usersテーブル

| Column   | Type   | Options     |
| -------- | ------ | ----------- |
| name     | string | null: false |
| email    | string | null: false |
| password | string | null: false |

## roomsテーブル

| Column | Type   | Options     |
| ------ | ------ | ----------- |
| name  | string | null: false |

## room_usersテーブル

| Column  | Type    | Options                        |
| ------- | ------- | ------------------------------ |
| user_id | integer | null: false, foreign_key: true |
| room_id | integer | null: false, foreign_key: true |

## messagesテーブル

| Column  | Type    | Options                        |
| ------- | ------- | ------------------------------ |
| content    | string  |
| user_id | integer | null: false, foreign_key: true |
| room_id | integer | null: false, foreign_key: true |

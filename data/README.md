# Data Dictionary

Gym data from [Kaggle](https://www.kaggle.com/datasets/mexwell/gym-check-ins-and-user-metadata)

## User Data

| field | description | cleaning notes |
| ------| ----------- | -------------- |
| user_id | int | PK  |
| first_name | str |  |
| last_name | str |  |
| age | int |  |
| gender | str |  |
| birthdate | date - format is YYYY-MM-DD |  |
| sign_up_date | date - format is YYYY-MM-DD |  |
| user_location | str |  |
| subscription_plan | str | FK |

## Subscription Plans

| field | description | cleaning notes |
| ------| ----------- | -------------- |
| subscription_plan | str | PK |
| price_per_month | float .2 |  |
| features | str |  |

## Gym Locations 

| field | description | cleaning notes |
| ------| ----------- | -------------- |
| gym_id | str | PK |
| location | str |  |
| gym_type | str |  |
| facilities | str |  |

## Checkin/Checkout History

| field | description | cleaning notes |
| ------| ----------- | -------------- |
| user_id | int |  |
| gym_id | str |  |
| checkin_time | date - format is YYYY-MM-DD time is 00:00:00 |  |
| checkout_time | date - format is YYYY-MM-DD time is 00:00:00 |  |
| workout_type | str |  |
| calories_burned | int |  |

 
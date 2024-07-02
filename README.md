classDiagram
    class User {
        +int id
        +string name
        +string email
        +string password
    }

    class Income {
        +int id
        +int user_id
        +float amount
        +string type
        +string frequency
        +string notes
        +date created_at
    }

    class Expense {
        +int id
        +int user_id
        +float amount
        +string type
        +string frequency
        +string notes
        +date created_at
    }

    class SavingsGoal {
        +int id
        +int user_id
        +string item
        +float goal_amount
        +float allocation_percentage
        +float monthly_income
        +date created_at
        +date forecasted_end_date
    }

    User --> Income: has
    User --> Expense: has
    User --> SavingsGoal: sets

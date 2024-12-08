# TripleTen Sprint 3 Project - Statistical Data Analysis(SDA)

This is the 3rd project I worked on in the TripleTen Data Science program. This project was an independent project, which was reviewed by officials of the program.

### Megaline Phone Plans

The goal of this project was to preprocess & analyze the data in order to conduct a hypothesis test that gave insight into clients' behavior and determine which prepaid plan brought in more revenue.

#### The Data

The data was spread across five files:

- `megaline_calls.csv`: table focused on calls made (each row held this information for each user)
    - `'id'`: ID number that uniquely identifies each call
    - `'user_id'`: ID number that uniquely identifies each user making the call
    - `'call_date'`: date that the call was made
    - `'duration'`: duration of the call (in minutes)
- `megaline_internet.csv`: table focused on web sessions/web traffic (each row held the monthly amount of mb used for each user)
    - `'id'`: ID number that uniquely identifies each web session
    - `'user_id'`: ID number that uniquely identifies the user of data/web usage
    - `'mb_used'`: volume of data spent during the month (in megabytes)
    - `'session_date'`: monthly web session date
- `megaline_messages.csv`: table focused on number of text messages sent per month (each row held the monthly number of texts made by each user)
    - `'id'`: ID number that uniquely identifies each text
    - `'user_id'`: ID number that uniquely identifies the user sending the text
    - `'message_date'`: the date of the text message
- `megaline_plans.csv`: table focused on both plan offered by Megaline
    - `'plan_name'`: name of phone plan
    - `'usd_monthly_fee'`: monthly charge in US dollars
    - `'minutes_included'`: monthly minute allowance
    - `'messages_included'`: monthly text allowance
    - `'mb_per_month_included'`: data volume allowance (in megabytes)
    - `'usd_per_minute'`: price per minute after exceeding the package limits (e.g., if the package includes 100 minutes, the 101st minute will be charged)
    - `'usd_per_message'`: price per text after exceeding the package limits
    - `'usd_per_gb'`: price per extra gigabyte of data after exceeding the package limits (1 GB = 1024 megabytes)
- `megaline_users.csv`: table focused on information related to users
    - `'user_id'`: ID number that uniquely identifies each user
    - `'first_name'`: user's name
    - `'last_name'`: user's last name
    - `'age'` — user's age (years)
    - `'reg_date'`: subscription date (dd, mm, yy)
    - `'churn_date'`: the date the user stopped using the service (if the value is missing, the calling plan was being used when this database was extracted)
    - `'city'`: user's city of residence
    - `'plan'`: calling plan name

#### The Process

I started by examining each dataset, addressing missing and duplicate values, and converting columns to the correct data types. I then aggregated tables to identify patterns in client behavior, which I visualized. Finally, I conducted statistical tests to compare the average revenue between the Ultimate and Surf plans and to determine if the NY-NJ area differed from other regions.

### Results

Taking the time to explain my results at each step was a key element in this process. I wrote an introduction and conclusion that outlined what I did, and gave Megaline more insight into their plans.

Please have a look at the Jupyter Notebook included for a full description of results.

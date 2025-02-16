# Megaline Revenue Showdown Surf vs. Ultimate
View project: [Megaline Revenue Showdown: Surf vs. Ultimate](https://github.com/BradyQuack/Megaline-Revenue-Showdown-Surf-vs.-Ultimate/blob/main/MegalineFinal.ipynb)
# Project description
You work as an analyst for the telecom operator Megaline. The company offers its clients two prepaid plans, Surf and Ultimate. The commercial department wants to know which of the plans brings in more revenue in order to adjust the advertising budget. You are going to carry out a preliminary analysis of the plans based on a relatively small client selection. You'll have the data on 500 Megaline clients: who the clients are, where they're from, which plan they use, and the number of calls they made and text messages they sent in 2018. Your job is to analyze clients' behavior and determine which prepaid plan brings in more revenue. 

## Description of the plans
### Surf

Monthly charge: $20

500 monthly minutes, 50 texts, and 15 GB of data

After exceeding the package limits:

1 minute: 3 cents

1 text message: 3 cents

1 GB of data: $10

### Ultimate

Monthly charge: $70

3000 monthly minutes, 1000 text messages, and 30 GB of data

After exceeding the package limits:

1 minute: 1 cent

1 text message: 1 cent

1 GB of data: $7

## Description of the data
### The users table (data on users):

user_id — unique user identifier 

first_name — user's name

last_name — user's last name

age — user's age (years)

reg_date — subscription date (dd, mm, yy)

churn_date — the date the user stopped using the service (if the value is missing, the calling plan was being used when this database was extracted)

city — user's city of residence

plan — calling plan name


### The calls table (data on calls):

id — unique call identifier

call_date — call date

duration — call duration (in minutes)

user_id — the identifier of the user making the call


### The messages table (data on texts):

id — unique text message identifier

message_date — text message date

user_id — the identifier of the user sending the text


### The internet table (data on web sessions):

id — unique session identifier

mb_used — the volume of data spent during the session (in megabytes)

session_date — web session date

user_id — user identifier


### The plans table (data on the plans):

plan_name — calling plan name

usd_monthly_fee — monthly charge in US dollars

minutes_included — monthly minute allowance

messages_included — monthly text allowance

mb_per_month_included — data volume allowance (in megabytes)

usd_per_minute — price per minute after exceeding the package limits (e.g., if the package includes 100 minutes, the 101st minute will be charged)

usd_per_message — price per text after exceeding the package limits

usd_per_gb — price per extra gigabyte of data after exceeding the package limits (1 GB = 1024 megabytes)

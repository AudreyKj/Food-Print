# Athena October 2022 Hackathon - FoodPrint

Our submission for the Athena Hcakathon in October 2022 on the theme "How can households reduce their carbon footprint?".

FoodPrint is a web app that scans food receipts and detects high carbon footackles food consumption's impact on carbon footprint emissions.

## App Features
- Scans users’ groceries receipt to calculate the food items’ carbon footprint 
- Sends reminders to users to avoid food waste
- Awards points for low carbon footprint food consumption to encourage users 
- Tracks previous receipts’ scans to help users’ track their impact

We use an OCR API to detect text in the receipt image and take into account the seasonality and type of the food items to calculate their carbon footprint.

We built our app with the security of our users in mind: we use cookie session for authentication and hash users' passwords with bycryptjs before storing them in the database. 

## Future improvements
- Implementing reminders via mobile messaging (SMS, WhatsApp, Telegram)
- Connecting users to local food producers with search and messaging features

## Hackathon 
We teamed up for the Hackathon and had a great time imagining and building this app from scratch in only 35 hours!

## Tech stack
React, Node.js, Express, PostgreSQL, OCR API <br />

## Local installation 

- Clone the repository 

- Install dependencies 
```bash
npm install
```

- Set up a PostgreSQL database:

Set up a PostgreSQL database (download [PostgreSQL](https://www.postgresql.org/download/) if necessary) and add the database credentials in a `.env` file. Once the database is created, connect to your database `psql -d databaseName`, and create the tables found in `database/tables`.

- Run a development server:

Concurrently in 2 different tabs:
```bash
npm start
```

```bash
cd client 
npm start
```

## Credits
Audrey (developer), Sowjanya(developer), Kate (developer), Nadia (designer), Adeola (designer)

## Screenshots 

!['home'](home.png)
!['register'](register.png)
!['login'](login.png)
!['dashboard'](dashboard-1.png)
!['dashboard'](dashboard-2.png)
!['dashboard'](dashboard-3.png)
!['receipts'](receipts.png)
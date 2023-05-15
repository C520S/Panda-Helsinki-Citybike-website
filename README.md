# Panda Helsinki Citybike website



# ****Description****



I developed this web application as a pre-assignment for the Solita Development Academy in Finland in 2023. It contains comprehensive data on bike-share trips in the Helsinki and Espoo areas for the month of May 2021. Our app offers a range of statistics on user trips, such as station addresses, capacity, number of pick-ups and drop-offs, and average distance between stations. Our user-friendly table format enables easy comparison of statistics from different stations. We have also included a map displaying the location of each station, so you can view the bike stations in their geographic context. Our objective is to furnish an intuitive interface that allows you to access and explore the data with ease.

# Demonstration



- Project presentation video : [https://youtu.be/K4-qSEnbT8E](https://youtu.be/K4-qSEnbT8E)
- Web link: [https://panda-helsinki-citybike-website.onrender.com](https://panda-helsinki-citybike-website.onrender.com/)

# ****Features****



## Front End

- Good user interface design with a panda theme and focus on colour balance
- The homepage uses a carousel to showcase pandas and describe the site.
- Includes a navigation bar to allow the user to switch between the Journey and Station pages and the Home Page.
- The journey page has a good table displaying the content of the data The display includes the departure place, departure time (in the form of day-month-year), return place, return time (in the form of day-month-year), distance covered (in km) and duration (in min).
- The data in the table on the journey page can be sorted.
- The data in the table on the journey page can be paginated.
- The data in the table on the journey page can be searched and paginated by using the name of the departure station.
- Ignore upper and lower case letters when searching for a station name on the Journey page - if the station name does not exist, a prompt will appear to remind you to enter the station name you require.
- The station page has a nice table that shows the content of the data. The display includes the station name, the bike capacity, the city and the address.
- The data in the table on the station page can be sorted.
- The data in the table on the station page can be paginated.
- The data in the table on the station page can be searched and paginated by using the name of the station.
- Ignore upper and lower case letters when searching for a station name on the Station page - if the station name does not exist, a prompt will appear to remind you to enter the station name you require.
- Station details can be accessed by clicking on the station name.
- The single station view page has a nice table showing the data content, which includes a map (the location is marked on the map and if you click on the panda icon, the name of the station is displayed), the station identification number, the name of the station, the address of the station, the city and operator, the bike capacity, the average distance in km starting from the station and the average distance in km ending at the station, the total number of journeys starting from the station, the total number of journeys ending at the station, the top 5 most popular stations for journeys starting from the station, the top 5 most popular stations for journeys ending at the station.
- If the user enters an incorrect URL address it will go to a 404 page.
- Front end is deployed on the cloud

## **Backend**

- Removes data containing blank fields, negative values, distances under 10m and durations under 10s.
- The data was saved in the MongoDB Atlas database.
- Backend is deployed on the cloud
- I make REST APIs for front-end applications to use, here is the documentation link to the API [Panda Bicycle API Documentation.pdf - Google Drive](https://drive.google.com/file/d/1Xvw0rxSChzQVDUK6z9_DkUUDnMV2bjlH/view)

# Automation Testing



## End-to-end testing

Here is the end-to-end test report :

[https://drive.google.com/file/d/1RURlokEed0QEqtNlCEcy_gr-y-q-jL7T/view?usp=sharing](https://drive.google.com/file/d/1RURlokEed0QEqtNlCEcy_gr-y-q-jL7T/view?usp=sharing)

## REST APIs Testing

Here is the test report for the REST APIs :

[https://drive.google.com/file/d/1svHIOZjx_m_4-p1REVDiqjq84xrgm49E/view?usp=sharing](https://drive.google.com/file/d/1svHIOZjx_m_4-p1REVDiqjq84xrgm49E/view?usp=sharing)

# **Technology choices**



## Front End

- **React**
- **And design**
- **JavaScript**
- **HTML**
- **CSS**

## **Backend**

- **Node**
- **Express**
- **JavaScript**

## **Database**

- **MongoDB Atlas**

## End-to-end testing

- **Playwright**
- **Node**
- **TypeScript**

## REST APIs Testing

- **Node**
- **Mocha**
- **Chai**
- **JavaScript**
- **JSON Schema**

# Bicycle data



## **Journey details**

- [https://dev.hsl.fi/citybikes/od-trips-2021/2021-05.csv](https://dev.hsl.fi/citybikes/od-trips-2021/2021-05.csv)

## Helsinki Region Transport’s (HSL) city bicycle stations

- Dataset: [https://opendata.arcgis.com/datasets/726277c507ef4914b0aec3cbcfcbfafc_0.csv](https://opendata.arcgis.com/datasets/726277c507ef4914b0aec3cbcfcbfafc_0.csv)
- License and information: [https://www.avoindata.fi/data/en/dataset/hsl-n-kaupunkipyoraasemat/resource/a23eef3a-cc40-4608-8aa2-c730d17e8902](https://www.avoindata.fi/data/en/dataset/hsl-n-kaupunkipyoraasemat/resource/a23eef3a-cc40-4608-8aa2-c730d17e8902)

# Code Repository



- Front-end code :              [https://github.com/C520S/front-end.git](https://github.com/C520S/front-end.git)
- Back-end code:                [https://github.com/C520S/backend.git](https://github.com/C520S/backend.git)
- End-to-end code:             [https://github.com/C520S/E2E-tests.git](https://github.com/C520S/E2E-tests.git)
- REST APIs Testing Code : [https://github.com/C520S/api-testing.git](https://github.com/C520S/api-testing.git)

# **Author**



- [https://github.com/C520S?tab=repositories](https://github.com/C520S?tab=repositories)

# ****Usage and Installation****



## Front-end code

1. Clone or download to your local PC
2. npm install
3. npm start

## Back-end code

1. Clone or download to your local PC
2. npm install
3. npm start

## End-to-end code

1. Clone or download to your local PC
2. npm install
3. npx playwright install
4. View the report: **npx playwright show-report**
5. Run e2e tests: **npm run test:e2e**
6. Run e2e tests and demonstrate Google Chrome: **npm run test:e2eWithBrowser**
7. Run e2e tests and make reports: **npm run test:e2e-reporter**

## REST APIs Testing Code

1. Clone or download to your local PC
2. npm install
3. Run API tests : **npm run test:Api**
4. Run API tests and make reports : **npm run test:Api-reporter**

# FAQ



While using the free version of MongoDB Atlas, I was experiencing issues with having to run on a shared CPU and limited cluster space. To optimise the responsiveness of my web pages and improve the overall user experience, I decided to upload only one dataset of journey details to the database.


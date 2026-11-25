# Mikita Skrabneuski


![Profile](/rsschool-cv/images/profile.jpg "Profile")


*Minsk, Belarus*

---


## Contact

***nskrabnevsky@gmail.com***

---


## Profile


> My goal is to become a professional in full-stack development. I completed an internship as a Salesforce Developer, where I created web forms, LWC components, Apex classes, triggers, created API endpoints, developed integrations using MuleSoft. Also, I participated in the TMS FrontEnd course, where I learned basics of FrontEnd development from HTML to React, Redux, and RTK Query.

---


## Skills


`Git` `Markdown` `HTML` `CSS` `Tailwind` `Bootstrap` `Javascript` `Typescript` `React` `Redux` `RTK Query` `API` `Postman` `Node.js` `Express` `Salesforce` `Apex` `LWC` `Firebase`

---

## Code example

[Create API service using RTK Query](https://github.com/nikskr/weather-frontend-app/blob/dev/src/service/WeatherService.ts)


```
import { createApi, fetchBaseQuery } from "@reduxjs/toolkit/query/react";
import { type ICityForecast, type ILocationCurrentWeather } from "../models/IWeather";

export const weatherAPI = createApi({
    reducerPath: 'currentWeatherAPI',
    baseQuery: fetchBaseQuery({ baseUrl: import.meta.env.VITE_BASE_API_URL }),
    endpoints: (builder) => ({
        fetchCurrentWeatherByLocation: builder.query<ILocationCurrentWeather, string>({
            query: (location) => ({
                url: '/current.json',
                params: {
                    q: location,
                    key: import.meta.env.VITE_WEATHER_API_KEY
                }
            })
        }),
        fetchForecastByLocation: builder.query<ICityForecast, string>({
            query: (location) => ({
                url: '/forecast.json',
                params: {
                    q: location,
                    key: import.meta.env.VITE_WEATHER_API_KEY,
                    days: 14
                }
            })
        })

    })
})
```

---


## Work experience


* [Weather App](https://nikskr.github.io/weather-frontend-app/) - 
    [GitHub](https://github.com/nikskr/weather-frontend-app) - 
    `Git` `Typescript` `React` `Vite` `Redux`
* [Posts App](https://nikskr.github.io/posts-react-app/) - 
    [GitHub](https://github.com/nikskr/posts-react-app) - 
    `Git` `Javascript` `React` `Axios`
* [Store Page](https://nikskr.github.io/abito-app/) - 
    [GitHub](https://github.com/nikskr/abito-app) - 
    `Git` `HTML` `CSS` `JS`

---


## Education


- *2022* - **BSUIR** - Bachelor's degree
- *2024* - **BSUIR** - Master's degree

---

## English - ***B1***

> I have advanced reading skills, and intermediate listening and writing skills. I am working on my speaking.

---

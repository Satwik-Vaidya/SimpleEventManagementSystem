# Event Booking System

A full-stack web application for managing event bookings, built with Node.js, Express, MySQL, and EJS templating.

## Features

- **User Management**: Registration and authentication for users
- **Event Organization**: Create and manage events with details like venue, date, and ticket pricing
- **Booking System**: Users can book tickets for events
- **Rating System**: Rate attended events
- **Ticket Management**: View and cancel bookings
- **Organizer Dashboard**: Track bookings and event statistics

## Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: MySQL
- **Templating**: EJS
- **Authentication**: Custom implementation (passwords stored as plaintext - see security notes)

## Prerequisites

- Node.js (v16 or higher)
- MySQL 8.0+
- npm

---

## Database Schema

The system uses 5 main tables:

- **user**: Stores user information (userid, name, username, password, contact, age, email, address)
- **organiser**: Event details (eventid, eventname, eventdate, ticketprice, venuename, etype, econtact)
- **venue**: Venue information (venueid, venuename, address, capacity, food/beverages, venueowner)
- **booking**: Booking records linking users to events
- **rating**: Event ratings from users

## Security Considerations

> **Warning**: This is a development/demo project with several security concerns:


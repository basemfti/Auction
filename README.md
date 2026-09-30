# 🔨 Auction — Online Auction Platform

A full-stack online auction web application built with **Python, Django, SQLite, HTML, CSS, and JavaScript**.

The application allows users to create auction listings, place bids, add listings to a watchlist, comment on listings, and manage their own auctions.

This project was developed as part of **CS50's Web Programming with Python and JavaScript (CS50W)**.

---

## 📸 Overview

Auction provides an e-commerce-style platform where users can create and participate in online auctions.

Users can:

- Create auction listings
- Browse active listings
- Place bids
- Add listings to a watchlist
- Comment on listings
- View listing details
- Close auctions
- View their own listings
- Track their activity

---
## 🎥 Project Demo

Watch the video demonstration to see how the Auction platform works.

[![Auction Platform Demo](https://img.youtube.com/vi/bnfcbeBKQlQ/0.jpg)](https://www.youtube.com/watch?v=bnfcbeBKQlQ)

▶️ [Watch the full demo on YouTube](https://www.youtube.com/watch?v=bnfcbeBKQlQ)
## 🚀 Features

### 👤 User Authentication

- User registration
- Login and logout
- Session-based authentication
- User-specific actions

### 🔨 Auction Listings

Users can create listings containing:

- Title
- Description
- Starting bid
- Image
- Category

Users can browse active auction listings and view detailed information about each item.

### 💰 Bidding

Users can place bids on active listings.

The application validates bids before accepting them and ensures that a new bid meets the required conditions.

### ⭐ Watchlist

Users can add auction listings to their personal watchlist.

This allows them to easily return to auctions they are interested in.

### 💬 Comments

Users can leave comments on auction listings and view comments from other users.

### 🏆 Auction Closing

The owner of an auction can close the listing.

Once an auction is closed, the highest valid bidder becomes the winner.

### 📂 Categories

Listings can be organized into categories, making it easier for users to discover items.

---

## 🛠️ Technologies

| Technology | Purpose |
|---|---|
| Python | Backend programming |
| Django | Web framework |
| SQLite | Database |
| HTML5 | Page structure |
| CSS3 | Styling |
| JavaScript | Client-side functionality |
| Bootstrap | UI components |
| Django Templates | Dynamic HTML rendering |

---

## 🏗️ Application Architecture

```text
                    ┌─────────────────┐
                    │      User       │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │   Django Web    │
                    │   Application   │
                    └────────┬────────┘
                             │
              ┌──────────────┼──────────────┐
              │              │              │
              ▼              ▼              ▼
         Authentication   Auctions       Watchlist
              │              │              │
              └──────────────┼──────────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │     SQLite      │
                    │     Database    │
                    └─────────────────┘

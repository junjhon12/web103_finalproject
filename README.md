# TackleLog

CodePath WEB103 Final Project

Designed and developed by: Quoc Bao Le, Phuong Nguyen

🔗 Link to deployed app:

## About

### Description and Purpose

Full-stack fishing journal that lets anglers record every trip, log each catch, and track which lures actually produced fish.

### Inspiration

I like fishing

## Tech Stack

Frontend: React, Tailwind CSS, Fetch API

Backend: Node.js + Express, PostgreSQL, CORS + dotenv

## Features

### Trip Log

Create, view, edit, and delete fishing trips. Each trip stores location, date, weather, water temperature, and notes, and shows all catches from that day.

[gif goes here]

### Catch Tracking 

Log every fish with species, weight, length, time caught, and released/kept status. Catches support all four REST operations: view, create, update, and delete.

[gif goes here]

### Tackle Box with Lure Linking

A visual grid of every lure in your box, with a count of how many catches it's tied to. 

[gif goes here]

### [ADDITIONAL FEATURES GO HERE - ADD ALL FEATURES HERE IN THE FORMAT ABOVE; you will check these off and add gifs as you complete them]

## Installation Instructions

git clone https://github.com/junjhon12/tacklelog.git
cd tacklelog

# backend
cd server
npm install

# frontend
cd ../client
npm install

createdb tacklelog

psql tacklelog < server/db/schema.sql

DATABASE_URL=postgres://localhost:5432/tacklelog
PORT=3001

VITE_API_URL=http://localhost:3001

cd server
npm run dev

# in another terminal
curl -X POST http://localhost:3001/api/reset

# Might change later so that both front andb ack can be lauanch with one command

# backend
cd server
npm run dev

# frontend
cd client
npm run dev
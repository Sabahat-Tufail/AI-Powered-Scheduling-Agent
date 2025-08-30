# AI Calendar Assistant

## Overview

AI Calendar Assistant is an intelligent scheduling tool built with n8n and integrated with Google Calendar. It helps users check availability, manage events, and handle bookings through natural language queries.

## Features

* Check available/free time slots within a given time range
* Identify booked slots with clear responses
* Create and manage calendar events
* Natural language queries for ease of use
* Integrated with Google Calendar using n8n workflows

## Tech Stack

* **n8n**: Workflow automation engine
* **Google Calendar API**: For event scheduling and availability checks
* **Custom AI Agent**: Handles natural language queries and decision-making

## How It Works

1. User enters a natural language query (e.g., "What times am I free tomorrow between 9 AM and 6 PM?").
2. The AI Agent processes the query and extracts the required parameters (date, time range, intent).
3. The workflow calls the Google Calendar API to check for existing events.
4. A structured response is generated:

   * If events exist → Booked slots are displayed.
   * If no events exist → Available slots are displayed.

## Example Queries

* "Am I free between 2 PM and 4 PM tomorrow?"
* "List my meetings on September 5th."
* "Create an event with Ali at 3 PM on Monday."

## Project Structure

* `n8n Workflow`: Contains the automation flow logic
* `AI Agent`: Handles intent extraction and response formatting
* `Google Calendar Integration`: Manages API calls for event data

## Installation & Setup

1. Clone this repository.
2. Set up **n8n** on your local or cloud environment.
3. Connect Google Calendar credentials via n8n.
4. Import the workflow JSON file into your n8n instance.
5. Run the workflow and test queries.

## Future Improvements

* Support for recurring events
* Multi-user calendar integration
* Smart conflict resolution with suggestions



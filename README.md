# 📊 Snowflake Automated PDF Report Generator 📊

This is a quick proof of concept project to test out the functionality of Snowflake Notebooks. The goal was to limit myself to the main notebook functionality of the Snowflake Notebook envinronment as a way to learn. The idea was to create a scheduled dynamic report for a finctional business called WidgetCo. The end product is a daily automated report which sends a PDF report of daily sales to 3 different manages in the company all using the same report format but dynamically generating the data for each Manager and products A, B and C.

{{placeholder for demo video}}

## Features
- dynamically generated pdf reports for product lines A,B,C
- report can be visualized in notebook for testing
- dynamic email customized for each manager
- pdf reports are archived to an internal incase they need to be referenced later
- entire work flow is orchestrated from a single notebook that can be run adhoc or scheduled daily
- email failure altering, an email will be sent out if anyone of the reports fails to generate and send

## Requirements


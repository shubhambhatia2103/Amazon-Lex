# BankerBot with Amazon Lex

Welcome to the BankerBot project! This repository contains the code and documentation for creating a chatbot using Amazon Lex, designed to help a bank's customers check their account balances and transfer money between accounts.

## Project Overview

This project is divided into five parts, with the first part focusing on setting up a basic chatbot and configuring it to respond to user inputs. 

## Table of Contents

1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Setup Guide](#setup-guide)
4. [Creating Your First Intent](#creating-your-first-intent)
5. [Managing FallbackIntent](#managing-fallbackintent)
6. [Clean Up Resources](#clean-up-resources)
7. [Acknowledgments](#acknowledgments)

## Introduction

BankerBot is a practical chatbot built with Amazon Lex, which can help your bank's customers check their account balances and transfer money between accounts.

## Prerequisites

Before you begin, ensure you have the following:

- An AWS account
- Basic knowledge of AWS Console
- Familiarity with Amazon Lex

## Setup Guide

### Step 1: Set up your Lex chatbot

1. Login to your AWS Console and navigate to Amazon Lex.
2. Ensure you're in the Lex V2 console.
3. Select **Create bot** and then **Create a blank bot**.
4. Configure the bot with the following details:
   - **Bot name:** BankerBot
   - **Description:** Banker Bot to help customers check their balance and make transfers.
   - **IAM permissions:** Create a role with basic Amazon Lex permissions.
   - **COPPA:** No
   - **Idle session timeout:** 5 minutes
5. Choose your preferred voice for the bot.
6. Set the **Intent classification confidence score threshold** to 0.40.
7. Click **Done**.

### Step 2: Create Your First Intent

1. Name the intent `WelcomeIntent`.
2. Add the description: Welcoming a user when they say hello.
3. Add sample utterances:
   - Hi
   - Hello
   - I need help
   - Can you help me?
4. Define the closing response: "Hi! I'm BB, the Banking Bot. How can I help you today?"
5. Save and build the intent.
6. Test your bot with various phrases.

### Step 3: Manage FallbackIntent

1. Navigate to **FallbackIntent** in your Lex console.
2. Modify the closing response to: "Sorry I am having trouble understanding. Can you describe what you'd like to do in a few words? I can help you find your account balance, transfer funds, and make a payment."
3. Add variations to the response.
4. Save and build the intent.
5. Test the bot again to ensure it handles unrecognized inputs properly.

### Step 4: Clean Up Resources

To avoid any charges, make sure to delete your BankerBot:

1. Go to your Amazon Lex console.
2. Select **Bots** on the left-hand sidebar.
3. Choose **BankerBot** and select **Delete** from the Action drop-down.


## Acknowledgments

This project is part of a series by NextWork. Thank you for participating, and stay tuned for the next parts where we will enhance BankerBot's functionality further.

# ChatBot using ChatGPT API

A simple ChatBot project developed in Java using Spring Boot and integrated with ChatGPT API.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [API Endpoint](#api-endpoint)
- [Configuration](#configuration)
- [DTOs](#dtos)
- [Usage](#usage)
- [API Key](#api-key)

## Introduction
This project demonstrates a ChatBot application that uses the ChatGPT API to provide responses based on user input prompts. It's built using Java with Spring Boot and leverages Swagger for API documentation.

## Features
- Sends user prompts to ChatGPT API and retrieves responses.
- Uses Spring Boot's RESTful API architecture.
- Incorporates Swagger for API documentation.

## Tech Stack
- Java 8
- Spring Boot 2.5
- Maven for build and dependency management
- Dependencies used: Spring web and Lombok 


## Getting Started
1. Clone this repository.
2. Replace the values of `${openai.model}` and `${openai.api.url}` in `application.properties` with your actual ChatGPT API model and URL.
3. Build the project using Maven.
4. Run the Spring Boot application.

## API Endpoint
- Endpoint: `/bot/chat`
- Method: `GET`
- Request Parameter: `prompt` (User input prompt)

## Configuration
- `ChatBotController`: The main controller that handles user requests and interacts with the ChatGPT API.

## DTOs
- `ChatGPTRequest`: Represents the request to the ChatGPT API. Contains the model and messages.
- `ChatGPTResponse`: Represents the response from the ChatGPT API. Contains choices with indexes and messages.
- `Message`: Represents a message with role and content.

## Usage
1. Make a GET request to `/bot/chat` endpoint with the `prompt` parameter.
2. Receive the response from the ChatGPT API.

## API Key
To use this project, you'll need a ChatGPT API key. If the provided API key does not work or is expired, you can create your own API key by following the instructions provided by OpenAI. [Create ChatGPT API Key](https://openai.com/docs/guides/authentication).

# MoviesDatabase API Integration

This project integrates with the MoviesDatabase API to fetch and manage movie-related data. Below is the documentation for the API, including endpoints, authentication, and usage guidelines.

## API Overview

The MoviesDatabase API provides access to a comprehensive collection of movie data, including titles, release dates, ratings, cast, and more. Key features include:

- Fetching movie details by ID, title, or genre
- Searching for movies with filters (year, rating, etc.)
- Accessing actor/actress information
- Retrieving trending and upcoming movies

## Version

The current version of the API is **v1**.

## Available Endpoints

- `GET /titles` - Retrieve a list of movie titles with optional filters
- `GET /titles/{id}` - Get detailed information about a specific movie
- `GET /search` - Search for movies by title, genre, or keyword
- `GET /trending` - Fetch currently trending movies
- `GET /upcoming` - Retrieve upcoming movie releases
- `GET /actors` - Get information about actors/actresses
- `GET /actors/{id}` - Get detailed information about a specific actor

## Request and Response Format

### Request Format
All requests should include:
- `Content-Type: application/json` header
- API key in the `X-API-KEY` header

Example request:
```http
GET /titles/tt1234567 HTTP/1.1
Host: api.moviesdatabase.com
X-API-KEY: your-api-key-here
Content-Type: application/json
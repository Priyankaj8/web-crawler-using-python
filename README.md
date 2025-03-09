# Web Crawler using Python

## Overview
This is a simple web crawler built using Python that extracts links from web pages and saves them for further crawling. The crawler utilizes multi-threading for efficient web scraping and stores crawled links in a text file.

## Features
- Multi-threaded crawling for faster performance
- Extracts all valid links from web pages
- Saves queued and crawled links in text files
- Respects domain constraints to prevent crawling external websites

## Technologies Used
- Python
- `urllib.request` for fetching web pages
- `html.parser` for parsing HTML content
- `queue.Queue` for managing links
- `threading` for multi-threading support

## Project Structure
```
web-crawler/
│── spider.py           # Main crawling logic
│── link_finder.py      # Extracts links from HTML pages
│── domain.py           # Extracts domain name from URLs
│── demo.py             # Helper functions for file handling
│── main.py             # Entry point to start crawling
│── queue.txt           # List of URLs to be crawled
│── crawled.txt         # List of already crawled URLs
│── README.md           # Project documentation
```

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/web-crawler.git
   ```
2. Navigate to the project folder:
   ```sh
   cd web-crawler
   ```
3. Install dependencies (if any):
   ```sh
   pip install -r requirements.txt
   ```

## Usage
1. Update `HOMEPAGE` in `main.py` with the website you want to crawl.
2. Run the crawler:
   ```sh
   python main.py
   ```
3. The crawled URLs will be stored in `crawled.txt`, and pending links in `queue.txt`.

## Screenshot
![image](https://github.com/user-attachments/assets/6b7d16b6-052c-48d2-86e2-f69370a30764)  

## Notes
- Ensure that the target website allows web scraping by checking its `robots.txt` file.
- Use this tool responsibly and avoid overloading websites with too many requests.

## License
This project is licensed under the MIT License.

## Author
Priyanka J

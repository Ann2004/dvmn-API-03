# VK URL Shortener and Click Counter

This script allows users to shorten URLs using VK's link-shortening service and track the number of clicks on shortened links.

### How to install

Create a `.env` file in the project directory and add your VK access token:
```
VK_TOKEN=your_access_token
```

To use the VK API, you need an access token. [Create an application](https://id.vk.com/about/business/go/docs/ru/vkid/latest/vk-id/connection/create-application) and obtain an API token with necessary permissions.

Python3 should already be installed. 
Use `pip` (or `pip3`, if there is a conflict with Python2) to install dependencies:
```
pip install -r requirements.txt
```

### Usage
Run the script from the command line, providing a URL as an argument:
```
python main.py <your_link>
```

- If the provided link is a full URL, the script will shorten it.
- If the link is already shortened, it will return the number of clicks.

### Example Usage
To shorten a URL:
```
python main.py https://example.com
```
Output:
```
Сокращенная ссылка: https://vk.cc/abcd
```

To check the number of clicks on a shortened URL:
```
python main.py https://vk.cc/abcd
```
Output:
```
Количество кликов по ссылке: 42
```

### Project Goals

This code was written for educational purposes as part of an online course for web developers at [dvmn.org](https://dvmn.org/).

# 🌤️ Compostela Weather Updates Automation

### 📘 Overview
This project automates the process of generating and posting **real-time weather updates** for **Compostela, Cebu**, using **n8n** workflow automation.
It integrates **OpenWeatherMap API**, **OpenAI GPT-4**, and **Facebook Graph API** to create summarized, image-based weather reports that are automatically published on social media multiple times per day.

---

## ⚙️ Features
- ⏱️ **Automated Scheduling** – Posts updates every 6 AM, 12 PM, 6 PM, and 10 PM.
- ☁️ **Weather Data Integration** – Fetches live data from the **OpenWeatherMap API**.
- 🧠 **AI Summarization** – Uses **GPT-4** to create clear, concise weather summaries.
- 🖼️ **Dynamic Image Creation** – Adds weather data to image templates using **n8n Edit Image** node.
- 📤 **Auto Posting** – Publishes updates directly to **Facebook Pages** using **Graph API**.
- 📁 **Cloud Storage Integration** – Uses **Google Drive API** for image templates and asset management.

---

## 🧩 Tech Stack
| Category | Tools / Services |
|-----------|------------------|
| Automation Platform | n8n |
| Weather API | OpenWeatherMap |
| AI Text Generation | OpenAI GPT-4 |
| Image Editing | n8n Edit Image node |
| Cloud Storage | Google Drive API |
| Social Media Integration | Facebook Graph API |
| Scheduling | n8n Cron Trigger |

---

## 🛠️ Setup Instructions

### 1️⃣ Requirements
- n8n instance (self-hosted or cloud)
- OpenWeatherMap API key
- OpenAI API key
- Facebook Page Access Token (for posting)
- Google Drive credentials (for image access)

### 2️⃣ Import the Workflow
1. Open **n8n**.
2. Click on **Import Workflow** → Upload the provided `Compostela-Weather-Updates.json` file.
3. Review and connect the required credentials for each API node.

### 3️⃣ Configure Environment Variables
Set the following environment variables in your n8n settings or credential manager:
```bash
OPENWEATHERMAP_API_KEY=your_api_key_here  
OPENAI_API_KEY=your_openai_key_here  
FACEBOOK_PAGE_ACCESS_TOKEN=your_facebook_token_here  
GOOGLE_DRIVE_CREDENTIALS=your_google_credentials_here  
```

### 4️⃣ Run or Schedule
- Manually trigger the workflow to test.
- Enable the **Cron node** to automatically post updates at scheduled times.

---

## 🖼️ Example Output
**Sample Facebook Post:**  
> 🌤️ **Compostela, Cebu City** is currently experiencing a **warm and very humid atmosphere.**  
> With temperatures hovering around **25°C**, it feels quite muggy outside, making for a rather sticky day.  
> The skies are mostly cloudy, and the air is noticeably thick with just a gentle breeze. 💧☁️  
>
> **Location:** Compostela, Cebu City  
> **Temperature:** 24.93°C  
> **Humidity:** 97%  
> **Wind Speed:** 1.02 KM/H  
> **Wind Direction:** South  
> **Pressure:** 1007 MB  
>
> #CompostelaCebu #CebuWeatherUpdate #HumidFeels #CloudySkies #TropicalVibes


---

## 📸 Screenshots
🧭 Workflow Overview <img width="100%" alt="Workflow Overview" src="https://github.com/user-attachments/assets/c80e985e-f0b7-40dd-b4a7-7a856f6d3b1d" />

📱 Facebook Output <img width="1910" height="948" alt="image" src="https://github.com/user-attachments/assets/3cc76863-c4ae-4f7a-824c-15830db0c3cc" />


---

## 📈 Future Enhancements
- Add Twitter/X auto-posting.
- Store daily weather summaries in Google Sheets for history tracking.
- Include severe weather alert notifications.

---

## 👨‍💻 Author
**Arjun Rosell**  
📍 Cebu, Philippines  
💼 [LinkedIn](https://www.linkedin.com/in/rosellarjunp/)  
💻 [GitHub](https://github.com/rosellarjun)

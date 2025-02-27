# 📊 YouTube Trending Videos Analysis Dashboard

## Project Overview  
This project involves analyzing **trending YouTube videos** across **10 countries** over **205 days** using **Power BI**.  
The goal is to extract insights into trending content, audience engagement, and category performance, helping content creators and businesses optimize their strategies.  

### 📊 Dashboard Overview
Here is a preview of the Power BI dashboard:

<table>
  <tr>
    <td><img src="https://private-user-images.githubusercontent.com/190957386/417387530-d8473da5-f309-41e3-a3e0-105d9d5eb04c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDA2MjA3MzYsIm5iZiI6MTc0MDYyMDQzNiwicGF0aCI6Ii8xOTA5NTczODYvNDE3Mzg3NTMwLWQ4NDczZGE1LWYzMDktNDFlMy1hM2UwLTEwNWQ5ZDVlYjA0Yy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwMjI3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDIyN1QwMTQwMzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1iNTk3YTM2NmRhZmZlMWZlODE3ZDQ5N2VjZDk0Y2M4YjRjY2Y5NGUxZmQ2M2FjMjM2ODM4OTZhMDQwNTZmMjFkJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.zbVPTSC6sxMC5UXIXxs6tp34CTL5FsJiFjEpiUyRALI" width="400"></td>
    <td><img src="https://private-user-images.githubusercontent.com/190957386/417387532-65d8d14b-b2b2-496b-80de-6c873aec0cac.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDA2MjA3MzYsIm5iZiI6MTc0MDYyMDQzNiwicGF0aCI6Ii8xOTA5NTczODYvNDE3Mzg3NTMyLTY1ZDhkMTRiLWIyYjItNDk2Yi04MGRlLTZjODczYWVjMGNhYy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwMjI3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDIyN1QwMTQwMzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1kMGQzZjZiNzQ2Y2NiZWNiZjlkOWYzMjljZTRjOWQ4ZWZlNmFiN2NhOTUxNjE0YWFhYzZjMmM3YmY0NmJmYmViJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.EPIje7JvBTu1dX22Ur6GkKQemAPQFnq2DnGcTr8HsAg" width="400"></td>
  </tr>
  <tr>
    <td><img src="https://private-user-images.githubusercontent.com/190957386/417387531-abb705cd-a976-4d65-8b7d-d0dade558cdd.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDA2MjA3MzYsIm5iZiI6MTc0MDYyMDQzNiwicGF0aCI6Ii8xOTA5NTczODYvNDE3Mzg3NTMxLWFiYjcwNWNkLWE5NzYtNGQ2NS04YjdkLWQwZGFkZTU1OGNkZC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwMjI3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDIyN1QwMTQwMzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0yNDJhYWZhZmY4ODhhODJlODllZGI1NDZiMTU4NGE5YjAyMjZlZGUwMWI4Zjg2ZjJlYjJkNDAwNzZkNGIwOGM5JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.Oa4Y_sVnpaznrDVN8Mm58XDOxPNBXMZBev5zq7wqIYA" width="400"></td>
    <td><img src="https://private-user-images.githubusercontent.com/190957386/417387529-ec9c872f-35fb-41f6-9071-8a6dd5967f8c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDA2MjA3MzYsIm5iZiI6MTc0MDYyMDQzNiwicGF0aCI6Ii8xOTA5NTczODYvNDE3Mzg3NTI5LWVjOWM4NzJmLTM1ZmItNDFmNi05MDcxLThhNmRkNTk2N2Y4Yy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwMjI3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDIyN1QwMTQwMzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1iYTQwMTM0MmY4Y2U2NDAwMzI0Y2RkMDQ2YTk4ZWYwZjhjY2NkNGE3MmFkOTdhYWRmYzFjOGYyNjIyZmQ4MTI3JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.Kc2IvSOl_dATruUrIluhi7-Mb3rAN_VZngnAAXpDSoM" width="400"></td>
  </tr>
</table>

## Dataset  
The dataset was obtained from **Kaggle** and includes:  
- **10 CSV files** (each representing a country's trending videos).  
- **10 JSON files** (mapping category IDs to category names).
- Dataset link: https://www.kaggle.com/datasets/datasnaek/youtube-new

### Countries Covered:  
🇺🇸 USA | 🇬🇧 UK | 🇩🇪 Germany | 🇨🇦 Canada | 🇫🇷 France | 🇷🇺 Russia | 🇲🇽 Mexico | 🇰🇷 South Korea | 🇯🇵 Japan | 🇮🇳 India  

## Key Insights Provided by the Dashboard  
 **Trending videos by category** (Entertainment, News, Sports, etc.)  
 **Most popular YouTube channels**  
 **Top trending videos based on views, likes, and comments**  
 **Geographical distribution of trending videos**   
 **Upload time analysis** (by hour and day) 
 **Monthly trend analysis** to identify seasonal patterns  

## Implementation Steps  
1 **Extracted & merged data** from multiple CSV & JSON files.  
2 **Cleaned & preprocessed** the dataset by handling missing values and duplicates.  
3 **Designed an optimized data model** with fact & dimension tables for efficiency.  
4 **Built interactive visualizations** using Power BI to present insights.  

## Demo Video  
🎬 Check out the interactive dashboard in Google Drive: https://drive.google.com/file/d/1h48vHUfn1VlpolaQog-6XUoxJ_RNfKiG/view?usp=sharing
  

## Technologies Used  
- **Power BI** – for data modeling visualization & dashboard creation  


#!/bin/bash

# Ask for GitHub username
read -p "Enter your GitHub username: " USERNAME

# Create README.md
cat <<EOF > README.md

# 🌌 $USERNAME | Future Space Tech Engineer 🚀

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0B3D91,100:000000&height=200&section=header&text=Exploring%20Beyond%20Earth&fontSize=30&fontColor=ffffff"/>
</p>

---

## 🧠 About Me

⚡ Electrical & Electronics Engineer in the making  
🛰️ Dream: ISRO Scientist | Astronaut | Flying Forces  
🔬 Passion: IoT, Photonics, Space Tech  

---

## 🚀 Current Focus

- 🔧 Arduino & Robotics  
- 💻 C Programming  
- 🌌 Space Tech & Photonics  
- 🎯 ISRO / AFCAT Preparation  

---

## 🛠️ Tech Stack

\`\`\`yaml
Languages:
  - C
  - Python (learning)

Hardware:
  - Arduino
  - Sensors & IoT Modules

Tools:
  - GitHub
  - Figma
\`\`\`

---

## 🔬 Projects

- 🌡️ IoT Temperature & Humidity Monitor  
- 🚦 Smart Traffic Light System  
- 📡 Li-Fi Communication  
- 🤖 Robotic Arm  
- 🌍 AQI Monitoring System  

---

## 📈 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=$USERNAME&show_icons=true&theme=tokyonight"/>
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=$USERNAME&theme=tokyonight"/>
</p>

---

## 🎯 Goals

- 🛰️ Work with ISRO  
- 🚀 Build real-world tech  
- 💡 Master electronics + programming  

---

## ⚡ Fun Fact

> Building tech today that might fly beyond Earth tomorrow 🌍✨

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:000000,100:0B3D91&height=120&section=footer"/>
</p>

EOF

# Initialize git repo
git init
git add README.md
git commit -m "🚀 Added ISRO-themed profile README"

# Add remote repo
git remote add origin https://github.com/$USERNAME/$USERNAME.git

# Push to GitHub
git branch -M main
git push -u origin main

echo "✅ Done! Your ISRO-themed GitHub README is live 🚀"

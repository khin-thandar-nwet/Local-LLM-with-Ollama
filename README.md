# Local-LLM-with-Ollama
Local LLM with Ollama
Ollama
# Step1:Brew
brew --version
# Step2: Installation
brew install ollama
# Step3: Serve start
ollama serve
# Step4; new window
ollama pull qwen2.5:3b
# Step5 :Run Burmese LLM Test
ollama run qwen2.5:3b

Step 6: Test
>>> Hello
Hi! How can I help you today?
Step4:browser
http://localhost:11434/
 http://localhost:11434/api/tags

<br> Mac
<br> 
 |
<br> 
Ollama
<br> 
 |
 <br>
Qwen2.5 / Llama
<br> 
 |
 <br>
Open WebUI
<br> 
 |
 <br>
Browser Chat Interface
<br> 
 |
 <br> 
Burmese Documents (RAG)

# Step 5. Install Docker Desktop
<br>
WEB UI
<br>
Download docker
<br>
https://www.docker.com/products/docker-desktop/?utm_source=chatgpt.com
<br>
install docker

# Terminal
open -a Docker
<br>
docker ps
<br>
# Step 5: Run Open WebUI
docker run -d \ --name open-webui \ -p 3000:8080 \ -e OLLAMA_BASE_URL=http://host.docker.internal:11434 \ -v open-webui:/app/backend/data \ --restart unless-stopped \ ghcr.io/open-webui/open-webui:main
docker start open-webui

<img width="1253" height="708" alt="Screenshot 2026-07-11 at 10 39 02 PM" src="https://github.com/user-attachments/assets/03667596-2a0e-4b14-8f32-ac7488a98a8d" />
<img width="1392" height="901" alt="Screenshot 2026-07-11 at 10 40 01 PM" src="https://github.com/user-attachments/assets/721848d5-8f22-46f1-8a63-8554aab253cc" />

Requirements List for Creating Own LLM
1.Objective
2.Target Language
3.Target User
4.User cases
Q&A, ChatBot, Classification
5,Data Privacy
6.Performance Target
7.Deployment Model

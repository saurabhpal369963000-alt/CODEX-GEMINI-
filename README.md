# CODEX-GEMINI
import google.generativeai as genai
genai.configure(api_key="TERI-API-KEY-YAHA-DAALO")
model = genai.GenerativeModel("gemini-1.5-flash")

def ask_gemini(prompt):
    response = model.generate_content(prompt)
    return response.text

# Example: Buyer ne bola "mujhe python script chahiye"
print(ask_gemini("Python me 100 line ka WhatsApp bot script likho"))

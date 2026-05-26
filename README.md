#ToxCore

###Project Overview
*ToxCore is an AI-powered online toxicity detection and support platform. It analyzes user-submitted text comments for harmful content and provides an intelligent chatbot assistant to help users understand toxicity and stay safe online.

Key Features
Toxicity Analysis Engine

Classifies comments across 6 categories: toxicity, severe toxicity, obscene, threat, insult, and identity attack
Returns per-category confidence scores with a 0.5 threshold for flagging
Provides human-readable reasons explaining why content was flagged

ToxCore AI Chatbot

Floating chat widget embedded in the UI
Conversational assistant powered by an LLM, with full message history context
Helps users understand toxicity concepts and online safety

Real-time Results

Instant feedback with toxicity scores, top category, and a clean/harmful verdict
Smooth, responsive UI with loading animations and auto-scroll


Tech Stack
LayerTechnologyML Modelunitary/toxic-bert (BERT fine-tuned on Jigsaw dataset)ML FrameworkPyTorch + HuggingFace TransformersLLM (Chatbot)Google Gemini 2.5 Flash via google-generativeai SDKBackendPython (FastAPI implied by /api/chat endpoint structure)FrontendReact (with hooks), Tailwind CSSConfigpython-dotenv for API key managementComputeCUDA GPU / CPU fallback

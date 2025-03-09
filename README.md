# **Agno 101**

## **Theory**
- **Agno** (previously called **Phi Data**) is an **open-source** framework for building **AI agents** and **agentic AI applications**.
- It allows the creation of **multi-modal agents** that can:
  - Use **memory**
  - Integrate **external knowledge sources**
  - Connect with **various tools**
- **Comparison with LangGraph:**
  - Both **LangGraph** and **Agno** support complex workflows.
  - **LangGraph** provides **granular control**, while **Agno** allows agent creation with **fewer lines of code**.
  - In **Agno**, agents can be created **independently** and connected to solve problems.
  - You can attach **LLMs, tools, and external data sources** to each agent.
  - **Agno** is **faster** and offers **simpler monitoring** compared to LangGraph.

---

## **AGNO - Hands-On Setup**

### **Setup Environment**
1. **Create workspace:**
   ```bash
   mkdir agnoworkspace && cd agnoworkspace
   ```
2. **Create virtual environment with Conda:**
   ```bash
   conda create -p venv python=3.12
   conda activate venv/
   ```
3. **Create a requirements file (`requirements.txt`)** with required libraries 
   
4. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
5. **Navigate to the first example:**
   ```bash
   cd "1.Basic agents"
   ```

---

## **Code Examples**

### **1. Basic Agent (`app.py`)**
- Write a simple program to create an agent.
- Run:
  ```bash
  python app.py
  ```

### **2. Using Memory & Tools (`agent_memory.py`)**
- This script integrates:
  - **Agents**
  - **Knowledge Bases (KBs)**
  - **Tools**
- Refer to Agno's documentation for available **tools and KBs**:
  📌 [Agno Docs](https://docs.phidata.com/tools/introduction)
- Run:
  ```bash
  python agent_memory.py
  ```

### **3. Convert to Streamlit (`agent_memory1.py`)**
- Convert the above code to **Streamlit** using ChatGPT for quicker execution.
- Review/ understand the code from ChatGPT - debug and see if you can simpligy it 
- Modify the last secition: print method replacement for a structured output 
- Run:
  ```bash
  streamlit run agent_memory1.py
  ```

### **4. Multi-Agent System (`multiagents.py`)**
- Create multiple agents:
  - **Web Agent**
  - **Finance Agent**
  - **Agent Team** (to manage them)
- Run:
  ```bash
  python multiagents.py
  ```

### **5. Playground for Experimentation (`playground.py`)**
- This script is a **sandbox** for testing workflows before deployment.
- Run:
  ```bash
  python playground.py
  ```
- Output:
  ```
  INFO Starting playground on http://localhost:7777
  Playground URL: https://app.agno.com/playground?endpoint=localhost%3A7777  
  ```
- **Access the playground:**
  - Open the URL: `https://app.agno.com/playground?endpoint=localhost%3A7777`
  - In the **ENDPOINT FIELD** (top-right corner), enter:
    ```
    http://localhost:7777
    ```
  - This allows local testing before production deployment.

---

## **Summary**
✅ **Agno** simplifies AI agent development with **faster execution and easier monitoring**.
✅ It enables **multi-agent systems**, **tool integrations**, and **knowledge-based AI applications**.
✅ Compared to **LangGraph**, Agno requires **less code** and is **more streamlined for agent creation**.
✅ The **Playground** feature allows **safe experimentation** before production deployment.

---

Let me know if you need further refinements! 🚀


# 🎓 College Helpdesk Chatbot (IBM Watson Assistant)

This is an AI-powered college helpdesk chatbot built using IBM Watson Assistant.
It can answer queries related to:
- Courses
- Fees
- Admission
- Fallback for unknown questions

The chatbot is deployed through IBM Cloud Web Chat and can be embedded in any webpage.

---

## 🚀 Features
- Welcome Action
- Course/Fees/Admission actions
- Fallback action
- Web Chat deployment
- Conversation starters

---

## 📌 Technologies
- IBM Cloud
- IBM Watson Assistant
- Web Chat Integration
- HTML/CSS

---

## 📥 How to Use
1. Open the embed.html file in a browser  
2. The chatbot will load automatically  
3. Ask: “courses”, “fees”, “admission”, etc.

---

## 💻 Embed Code (replace your IDs)
```html
<script>
  window.watsonAssistantChatOptions = {
    integrationID: "282f3316-229f-4930-9eb3-07cc4ef76e48", // The ID of this integration.
    region: "au-syd", // The region your integration is hosted in.
    serviceInstanceID: "f0f86546-261b-487b-b5a8-6794831c8395", // The ID of your service instance.
    onLoad: async (instance) => { await instance.render(); }
  };
  setTimeout(function(){
    const t=document.createElement('script');
    t.src="https://web-chat.global.assistant.watson.appdomain.cloud/versions/" + (window.watsonAssistantChatOptions.clientVersion || 'latest') + "/WatsonAssistantChatEntry.js";
    document.head.appendChild(t);
  });
</script>
<script src="https://web-chat.global.assistant.watson.appdomain.cloud/loadWatsonAssistantChat.js"></script>

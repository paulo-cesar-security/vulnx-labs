<html>
   <Style>
     {
            rgba(255,255,255,0.03) 1px,
            transparent 1px,
            transparent 3px
        );
        pointer-events: none;
        mix-blend-mode: soft-light;
    }
</style>
</head>
<body class="scanlines">

<div class="terminal">
    <div class="text" id="text"></div>
    <div class="cursor">_</div>
</div>

<script>
const firstText = "Hi, I'm Paulo Cesar 👾";
const secondText = "Cybersecurity.";

const textElement = document.getElementById("text");

const wait = (ms) => new Promise(resolve => setTimeout(resolve, ms));

async function typeText(text, speed = 90) {
    for (let i = 0; i <= text.length; i++) {
        textElement.textContent = "> " + text.slice(0, i);
        await wait(speed + Math.random() * 60);
    }
}

async function deleteText(speed = 60) {
    while (textElement.textContent.length > 2) {
        textElement.textContent = textElement.textContent.slice(0, -1);
        await wait(speed + Math.random() * 40);
    }
}

async function loopAnimation() {
    while (true) {
        textElement.textContent = "> ";

        await typeText(firstText, 80);

        await wait(1000);

        await deleteText(55);

        await wait(400);

        await typeText(secondText, 90);

        await wait(1800);

        await deleteText(45);

        await wait(500);
    }
}

loopAnimation();
</script>

</body>
</html>
# Vulnx Labs
## Cybersecurity Portfolio

## 📊🚨 SOC analysis 

Projetos práticos utilizando SIEM Microsoft Sentinel e Splunk, Microsoft Entra ID, Microsoft Defender, Wireshark, Nmap e várias outras ferramentas, com foco em detecção de ataques, análise de logs, threat hunting e resposta a incidentes.
Inclui simulações de força bruta, password spraying, ataques à MFA, falhas em políticas de acesso e atividades pós-comprometimento:

[Acessar](https://github.com/paulo-cesar-security/cybersecurity-portfolio/tree/main/cybersecurity-analyst)

---

## 🔓🐞 Pentest 
Projetos de Pentest focados na identificação de vulnerabilidades, análise de segurança e simulação de ataques controlados para fortalecer a proteção de sistemas e aplicações.

[Acessar](https://github.com/paulo-cesar-security/cybersecurity-portfolio/tree/main/cybersecurity-analyst/pentest)

---

## 🔍🖥️ Digital Forensics 

Projetos de Investigação Forense Digital com foco em coleta, preservação e análise de evidências, incluindo análise de logs, dispositivos e reconstrução de atividades maliciosas:

[Acessar](https://github.com/paulo-cesar-security/cybersecurity-portfolio/tree/main/forense-analysis)

--- 

## 🕵️🌐 OSINT Investigations 

Projetos de Open Source Intelligence (OSINT) voltados à coleta e análise de informações em fontes abertas, com foco em identificação de perfis, rastreamento digital, correlação de dados e apoio a investigações de segurança:
 
[Acessar](https://github.com/paulo-cesar-security/cybersecurity-portfolio/tree/main/osint-analysis)

---

## Ferramentas e Tecnologias

* SIEM Microsoft Sentinel e Splunk
* Microsoft Entra ID
* Microsoft Defender
* Autopsy
* FTK Imager
* ExifTool
* SHA-256
* PowerShell
* Wireshark
* Nmap
* Kali Linux

## Contato

LinkedIn: https://www.linkedin.com/in/paulo-cesar-security

---

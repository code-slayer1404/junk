# junk


public/locales
  /en
    header.json
    navbar.json
    unitConverter.json
    caseConverter.json
    wordCounter.json
    jsonFormatter.json
    colorPicker.json
    qrGenerator.json
  /hi
    header.json
    navbar.json
    unitConverter.json
    caseConverter.json
    wordCounter.json
    jsonFormatter.json
    colorPicker.json
    qrGenerator.json


import i18n from "i18next";
import { initReactI18next } from "react-i18next";
import HttpBackend from "i18next-http-backend";
import LanguageDetector from "i18next-browser-languagedetector";

i18n
    .use(HttpBackend) // load translation files
    .use(LanguageDetector) // detect user language
    .use(initReactI18next) // connect with React
    .init({
        fallbackLng: "en",
        debug: true,
        interpolation: {
            escapeValue: false
        },
        backend: {
            loadPath: "/locales/{{lng}}/{{ns}}.json" // path to JSONs
        },
        ns: ["header", "navbar", "unitConverter", "caseConverter", "wordCounter", "jsonFormatter", "colorPicker", "qrGenerator"],
        defaultNS: "header"
    });

export default i18n;

thats how my i18 setup is.





////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////


🔧 Text & Data Tools
Base64 Encoder/Decoder

URL Encoder/Decoder

Hash Generator (MD5, SHA-1, SHA-256)

Lorem Ipsum Generator

Text Diff Checker

CSV to JSON Converter

SQL Formatter

🎨 Design & Color Tools
Gradient Generator

Box Shadow Generator

Font Preview Tool

Icon Resizer (multiple sizes)

Favicon Generator

📊 Development Tools
Regex Tester

JSON Validator

XML Formatter

Timestamp Converter

User-Agent Parser

HTTP Status Code Lookup

🔐 Security Tools
Password Generator

JWT Debugger

SSL Certificate Checker

Data URI Generator

📁 File & System Tools
File Size Converter (KB, MB, GB)

MIME Type Lookup

IP Address Lookup

UUID Generator

https://fdc.nal.usda.gov/api-guide
2w0tosgt0Z62RI1UpMuutUXvkrSJyGLWflxbqUTh

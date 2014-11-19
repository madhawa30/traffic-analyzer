Traffic Analyzer
================

This project is concerned in extracting useful information from a public Twitter feed using WSO2 CEP (Complex Event Processor) and several other natural language processing tools. Twitter feed is narrowed down to a particular account, @road_lk which is popular for posting free crowd sourced traffic alerts. Currently available @road_lk feed is used to train NLP models which are utilized for entity recognition. In real time scenario, users can view/search for road traffic from a web UI and also can subscribe for a location to receive traffic alerts regularly. As an overview, WSO2 ESB (Enterprise Service Bus) receives the real-time Twitter feed via streaming API and it is forwarded to WSO2 CEP to generate traffic information available in feed alerts. Custom Siddhi extensions and queries process these streams to generate traffic information according to user request and publish them back to web UI or to alerts.
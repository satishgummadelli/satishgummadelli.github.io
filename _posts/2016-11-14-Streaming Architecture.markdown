---
layout: post
title:  "Streaming Architecture"
permalink: "/StreamingArchitecture/definition"
date:   2016-11-14 15:39:33 +0000
categories: Streaming Architecture and Big Data
---
In this blog I will give outline of Streaming Architecture and what components are involved in Streaming Architecture.

## Why we need Streaming Architecture
In the past, Data is analysed in Batches (Batch Processing) and then Business predicts the trends of Business and does planning accordingly, with IoT (Internet of Things) and Micro Services Architecure quick insights into the Real time Data, Stream Processing became defacto for emerging and agile organizations.

## How to achive Streaming Architecture
Key Technology stack for Streaming Architecture are based on
  - Messaging
  - Stream Processing

### Messaging Systems
  Messaging Systems decouple systems and provide Asynchronous communication with fault tolerance and reliablity. There are many Messaging Systems  such as

  -  [Active MQ](http://activemq.apache.org/)
  -  [Rabbit MQ](https://www.rabbitmq.com/)
  -  [WebSpeher MQ](http://www-03.ibm.com/software/products/en/ibm-mq)
  -  [Apache Kafka](https://kafka.apache.org/)

All the above Messagin Systems (aka Messaging Brokers)  provide publish and subscribe messaging pattern, but Apache Kafka wins over others messaging systems when events rate is around 100K+ messages per second.

### Stream Processing
  Stream Processing is a method of continious computation that happens as data is flowing through the system.

  popular Stream Processing Frameworks
  
  -  [Apache Storm](http://storm.apache.org/)
  -  [Samza](http://samza.apache.org/)
  -  [Spark Streaming](http://spark.apache.org/streaming/)
  -  [kafka Streams](http://docs.confluent.io/3.0.0/streams/)

Streaming Architecure is achived when Stream Processing is applied on events/messages from Messaging Systems.


Data Integration -> aims to make Data available to all the Systems in an organization.

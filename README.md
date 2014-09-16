## Event Logistics Utility

This is a long-term project of EESTEC AGH Krakow, aimed to facilitate the logistics aspect of organisation of workshops.
NOTE: This is an early version of the documentation, many things may and will change over time.

### Name of the system
Integrated utility for facilitation of event organisation

### Definition of the problem
EESTEC - Electrical Engineering Students' European AssoCiation - is a non-profit student organization for Electrical Engineering and Computer Science students in Europe with over 50 branches in about 30 countries. It is a pre-professional organization that empathizes a broad skill-set such as dif soft skills, but also technical skills in various fields. 

Once in a while each local commitee(later called LC) organises workshops for foreign students which usually last about a week, which members of other LCs can apply to. Usually about 20 participants are chosen, but there are some in which many more people participate. Such events require some logistics, including venue reservation, departures and arrivals, participant supervision, schedule management and many more. Many LCs deal with it by developing specific procedures which are then followed by event organising committees. This, however, often results in repeating many tedious steps which could easily be automated or at least simplified. 

### Goal of the system
This system is being created in order to facilitate these procedures, by taking best practises from different LCs, automatising the processes and integrating them into one system. The whole organisational process is going to be managed entirely by this system.

### Functional requirements:
* participant supervision
 * 
* schedule management
 * create schedule
* venue management
 * 
 * attendence check by scanning QR codes

### Non-functional requirements:
* web client
* mobile client with support of as broad a device range as possible
* ease of adaptation to


### System architecture
The application backend will consist of a RESTful service, which will serve as the only communication means between client and server. It can be hosted separately from a web client.

The web client is going to be a single-page application, where the UI is rendered on the client-side by the browser - the goal of single-page applications is to provide a more fluid user experience similar to this in a desktop application. The web client will make requests to the aforementioned service and render the UI with the use of Backbone.js.

The mobile clients will be hybrid apps, where lots of web client code can be reused

#### Technolgies to be used
* web frontend
 * HTML5, CSS
 * CoffeeScript
 * Underscore.js, Backbone.js, Handlebars.js
* hybrid mobile client
 * Apache Cordova
* backend 
 * application framework - not yet decided - due to the target group, it should use technologies which are common across consumer hosting, so everyone can easily deploy the system on any hosting they have, thus the choice is limited and eventually comes down to Python vs Ruby
 * some common SQL database - preferably MySQL or PostgreSQL


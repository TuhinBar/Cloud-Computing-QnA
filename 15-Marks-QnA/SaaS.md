# Q. What is software-as-a-Service(SaaS) and what are the main characteristics of SaaS solution? Describes through a schematic diagram and necessary explanations how XML and SOA is used to implement an Open SaaS enviroment. [3 +3 + 9]

## Part 1

## *What is SaaS?*
Software as a service (or SaaS) is a way of delivering applications over the Internet—as a service. Instead of installing and maintaining software, you simply access it via the Internet, freeing yourself from complex software and hardware management.
SaaS applications are sometimes called Web-based software, on-demand software, or hosted software. Whatever the name, SaaS applications run on a SaaS provider’s servers. The provider manages access to the application, including security, availability, and performance.

## *The benefits of SaaS*
Increased efficiency and cost effectiveness are the reasons many businesses give for turning to cloud-based SaaS solutions. The advantages include:

### *Low setup and infrastructure costs*
You just pay for what you need with no capital expenditure that needs to be depreciated on your balance sheet over time.

### *Accessible from anywhere*
Just connect to the internet and you can work from wherever you need to be via desktop, laptop, tablet or mobile or other networked device.

### *Scalability*
You can adapt your requirements to the number of people who need to use the system, the volume of data and the functionality required as your business grows.

### *Industry leading service level agreements (SLAS) for uptime and performance*
So you have assurances that the software will be available to use when you need it – a difficult promise for in-house teams to make.

### *Automatic, frequent updates*
Providers offer timely improvements thanks to their scale and because they receive feedback about what their customers need. This frees up your IT department for other more business-critical tasks.

### *Security at the highest level required by any customer*
Because of the shared nature of the service, all users benefit from the security level that’s been set up for those with the highest need.

## Part 2

## *SaaS Characteristics*
A good way to understand the SaaS model is by thinking of a bank, which protects the privacy of each customer while providing service that is reliable and secure—on a massive scale. A bank’s customers all use the same financial systems and technology without worrying about anyone accessing their personal information without authorisation.

- A “bank” meets the key characteristics of the SaaS model:

### *Multitenant Architecture*
A multitenant architecture, in which all users and applications share a single, common infrastructure and code base that is centrally maintained. Because SaaS vendor clients are all on the same infrastructure and code base, vendors can innovate more quickly and save the valuable development time previously spent on maintaining numerous versions of outdated code.
### *Easy Customisation*
The ability for each user to easily customise applications to fit their business processes without affecting the common infrastructure. Because of the way SaaS is architected, these customisations are unique to each company or user and are always preserved through upgrades. That means SaaS providers can make upgrades more often, with less customer risk and much lower adoption cost.
### *Better Access*
Improved access to data from any networked device while making it easier to manage privileges, monitor data use, and ensure everyone sees the same information at the same time.
### *SaaS Harnesses the Consumer Web*
Anyone familiar with Amazon.com or My Yahoo! will be familiar with the Web interface of typical SaaS applications. With the SaaS model, you can customise with point-and-click ease, making the weeks or months it takes to update traditional business software seem hopelessly old fashioned.
### *SaaS Trends*
Organisations are now developing SaaS integration platforms (or SIPs) for building additional SaaS applications. The consulting firm Saugatuck Technology calls this the “third wave” in software adoption: when SaaS moves beyond standalone software functionality to become a platform for mission-critical applications.

SaaS is one of several cloud computing solutions for business IT issues. Other ‘as-a-Service’ options include:

- Infrastructure as a Service (IaaS) – the provider hosts hardware, software, storage and other infrastructure component
- Platform as a Service (PaaS)
- Everything as a service (XaaS) – which is essentially all the "aaS" tools neatly packaged together.
- The payment model for these kinds of services is typically a per-seat, per-month charge based on usage – so a business only has to pay for what they need, reducing upfront costs.

# Part 3


![image](https://user-images.githubusercontent.com/85868593/204097330-7cc37eb2-4bd5-4e78-9797-b3813803493c.png)
## *Cloud SaaS, SOA and Interoperability*
- US NIST (National Institute  of Standards and Technology) defines  Cloud Software-as-a-Service  (SaaS) as  a  capability  provided  to  the  consumer  to  use  the  provider’s applications  running  on  a  cloud  infrastructure.  
- The  applications  are  accessible  from various  client  devices  through  a  thin  client  interface  such  as  a  web  browser.  The consumer  does  not  manage  or  control  the  underlying  cloud infrastructure including network,  servers,  operating  systems,  storage,  or  even  individual  application capabilities,  with  the  possible  exception  of  limited  user-specific  application configuration  settings.
- The applications in the  cloud  may be as  simple  as a time zone  converter  performing  a  single  discrete  function,  or  as  complex  as  a  holiday packaging system performing a set of related business functions.  
- As mentioned earlier, SOA and Web services are the technologies, besides several others, from which cloud computing  has evolved. The cloud should  not be  looked at as  a  new  architecture  but instead as another option  of  storing  and  running  services within  SOA.
- In  addition  to  developing  a  cloud  based  on  service-oriented architecture, the individual software applications  deployed therein may themselves be service-oriented.   
- Figure 2 Software Services in a cloud interact through interfaces 
![image](https://user-images.githubusercontent.com/85868593/204097724-0db3c527-4231-416e-a27e-5aa48cbfbcd2.png)

- A cloud may host a  variety of software applications as cloud services which fulfill the business requirements of its  varied  customers. Based on the  requirements of  the customers  (or  service  consumers)  these software services in the cloud  may need  to interact  with  each  other.  This  interaction  is  accomplished  through  formal, standardized  interfaces  defined  using  WSDL.  

- As SOA promotes  intrinsic interoperability, the  SOA-based cloud architecture would have cloud software services that are inherently interoperable. The XML-based vendor-neutral communications framework, comprising  of WSDL,  SOAP and UDDI for defining,  publishing, and using the  services, would ensure interoperability among the  various  cloud  services  running  on  different  software  platforms  and  hardware architectures.  
- An  important  aspect  of SOA is the  separation of the  service interface (the what) from its implementation. 
- As a result, a client (which may be another service) need not be concerned with the implementation details of the service in order to  use  it. The service  implementation performs the necessary processing. 
- A change  in  the  implementation  of  the  service  does  not  prevent  the  client  from communicating with the service, so long as the interface remains the same. We  illustrate  this  with  the  help  of  an  example.  
- We  identify  two  services  –  an Online Hotel Reservation system (OHRS)  and Cab-On-Hire system (COHS) – in the cloud. A fictitious business enterprise, ABC hotel, subscribes to OHRS application in order to provide online services  to its  clients (customer and  hotel personnel) through its  website ABCHotel.com.  The  services  (functionalities)  enable  the  clients  to  book accommodation,  cancel  a  booking,  check  availability  status,  generate  reports  etc. XYZ  Cabs  is  another  fictitious  business  enterprise  which  subscribes  to  COHS application,  to  provide  online  services  to  its  clients  through  its  website XYZCabs.com. The COHS allows its clients (online customers and its staff) to book a cab  and  cancel  a  booking.  
- The  ABC  Hotel  also  hires  the  cabs  for  its  in-house customers from XYZ Cabs.  In  order to fulfill  the  additional functional requirements the two cloud services must be able to interact with each other. For example, the ABC Hotel  requires  determining  the  total  number  of  its  customers  hiring  the  cabs  on  a specific  day. In  an  SOA-based  cloud  this  interaction  is  enabled  through  an  XML-based communication framework that uses  SOAP messages, as depicted  in  Figure 3.  
- Figure 3 XML-based Interaction between the cloud SaaS
![image](https://user-images.githubusercontent.com/85868593/204097887-2da8a860-d1d2-427c-8acb-b866bbe7e858.png)

-  The  hotel  administrator  submits  a request,  from  one  of the  ABCHotel.com  web pages,  to  XYZCabs.com  to  determine  the  number  of  its  customers  availing  the  cab service  on a particular day.  
-  The HTTP request generated is routed  via a  controlling servlet  on the  ABCHotel.com  web server, which determines  that it needs to  retrieve the information (raw  data)  from XYZ Cabs.  The servlet obtains this  data by using  a web  service  client  implemented  by ABCHotel.com  developers.  This  client  uses  the web service interface published by XYZCabs.com to invoke  a method  on its  server that returns the required information. 
-  The method invocation is performed by creating an  XML  message  that  contains  the method  name  and  any  required  parameters  and then  sending  it  to  XYZCabs.com’s  server  using  the  SOAP  protocol.  The  value(s) returned by the  method call are then wrapped in another XML message and sent back to the ABCHotel.com’s web  client, which  extracts  the information that it  needs and uses a server-side script engine to render  it as HTML. The HTML is then  returned to the client’s  browser. The advantage of using XML instead of HTML is that  only raw data  is  required  to  be  transferred  which  does  not  include  presentation  markups, thereby reducing network traffic.  Also, the code  required to make  a request is much simpler than that required to extract data from an HTML page.

### Sources - [Part 3](https://www.researchgate.net/figure/ML-based-Interaction-between-the-cloud-SaaS_fig3_215913357) - [Part 2 and Part 1](https://www.salesforce.com/in/saas/)

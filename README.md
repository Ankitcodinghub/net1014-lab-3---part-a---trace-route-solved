# net1014-lab-3---part-a---trace-route-solved
**TO GET THIS SOLUTION VISIT:** [NET1014 Lab 3 – Part A – Trace Route Solved](https://www.ankitcodinghub.com/product/net1014-networking-principles-lab-solved-3/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;123928&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;NET1014  Lab 3 – Part A – Trace Route Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
MANUAL 3

Lab 3 – Part A – Trace Route

Objectives

 Determine network connectivity to a destination host.

 Trace a route to a remote server using tracert.

Background / Scenario

Data travels from a source end device to a destination device. Route tracing software lists the path traversed by this data.

This route tracing software is typically executed at the command line as:

tracert &lt;destination network name or end device address&gt;

(Microsoft Windows systems)

Or

traceroute &lt;destination network name or end device address&gt;

(UNIX, Linux systems, and Cisco devices, such as switches and routers)

Both tracert and traceroute determine the route taken by packets across an IP network. The tracert (or traceroute) tool is often used for network troubleshooting. By showing a list of routers traversed, the user can identify the path taken to reach a particular destination on the network or across internetworks. Each router represents a point where one network connects to another network and through which the data packet was forwarded. The number of routers traversed is known as the number of hops the data traveled from source to destination.

Command-line based route tracing tools are usually embedded with the operating system of the end device. This activity should be performed on a computer that has Internet access and access to a command line.

Required Resources

 PC with Internet access

Instructions

Part A.1: Determine Network Connectivity to a Destination Host

To trace the route to a distant network, the PC must have a working connection to the Internet. Use the ping command to test whether a host is reachable. Packets of information are sent to the remote host with instructions to reply. The PC measures whether each packet receives a response, and how long it takes for those packets to cross the network.

a. Navigate to the Command Prompt, enter ping www.cisco.com to determine if it is reachable.

b. Now ping one of the Regional Internet Registry (RIR) websites located in different parts of the world to determine if it is reachable:

Africa: www.afrinic.net

Australia: www.apnic.net

South America: www.lacnic.net

North America: www.arin.net

The website you selected will be used in the next part for use with the tracert command.

Part A.2: Trace a Route to a Remote Server Using Tracert

After you use ping to determine if your chosen websites are reachable, you will use tracert to determine the path to reach the remote server. Look closely at each network segment that is crossed.

Each hop in the tracert results displays the routes that the packets take when traveling to the final destination. The PC sends three ICMP echo request packets to the remote host. Each router in the path decrements the time to live (TTL) value by 1 before passing it onto the next system. To decrement is to count down. When the decremented TTL value reaches 0, the router sends an ICMP Time Exceeded message back to the source with its IP address and the current time. When the final destination is reached, an ICMP echo reply is sent to the source host.

Step 1: Trace a route to www.cisco.com.

At the prompt, trace the route to www.cisco.com.

In this example, the source host sends three ICMP echo request packets to the first hop (192.168.1.1) with the TTL value of 1. When the router 192.168.1.1 receives the echo request packets, it decrements the TTL value to 0. The router sends an ICMP Time Exceeded message back to the source. This process continues until the source host sends the last three ICMP echo request packets with TTL values of 8 (hop number 8 in the output above), which is the final destination. After the ICMP echo request packets arrive at the final destination, the router responds to the source with ICMP echo replies.

For hops 2 and 3, these IP addresses are private addresses. These routers are the typical

setup for point-of-presence (POP) of the ISP. The POP devices connect users to an ISP network.

Step 2: Trace a route to a RIR web site.

a. Now perform a tracert to one of the RIR web sites from the previous part.

Africa: www.afrinic.net

Australia: www.apnic.net

South America: www.lacnic.net

North America: www.arin.net

b. A web-based whois tool is found at http://whois.domaintools.com/. It can be used to determine the

domains traveled from the source to destination.

Question: List the domains below from your tracert results using a web-based whois tool, such as http://whois.domaintools.com/.

172.20.0.1

172.16.16.1

Lab 3 – Part B – My Protocol Rules

Objectives

 Relate computer network protocols to the rules that you use every day for various forms of communication.

 Define the rules that govern how you send and interpret text messages.

 Explain what would happen if the sender and receiver did not agree on the details of the protocol.

Background / Scenario

Before beginning to communicate with each other, we establish rules or agreements to govern the conversation. These rules, or protocols, must be followed for the message to be successfully delivered and understood. Among the protocol characteristics that govern successful human communication are:

• An identified sender and receiver

• Agreed upon method of communicating

• Common language and grammar

• Speed and timing of delivery

• Confirmation or acknowledgment requirements

The techniques that are used in network communications share these fundamentals with human conversations

Instructions

Think about the commonly accepted protocol standards for sending text messages to your friends. Fill out the chart on the next page with some of the rules that you follow when texting with friends and others. The first row has been filled in as an example.

Reflection

1. Now that you have documented the protocols that you use when sending and reading text messages, do you think that these protocols would be the same if you were texting with friends or with your parents and teachers? Explain your answer.

The protocol will be the same but the data will probably be different.

2. What do you think that the consequences would be if there were no agreed-upon protocol standards for different methods of communications?

We would not be able to communicate as there would be many issues with communication such as misunderstandings

3. Share your protocol rules with your classmates. Are there differences between your protocols and theirs? If so, could these differences result in misunderstanding of the messages?

If the protocols are not compatible, a misunderstanding of messages could result.

Lab 3 – Part C – Determine the MAC Address of a Host

Objectives

 Determine the MAC address of a Windows computer on an Ethernet network using the ipconfig /all command.

 Analyze a MAC address to determine the manufacturer.

Background / Scenario

Required Resources

• PC running Windows 10 with at least one Ethernet network interface card (NIC)

• Connectivity to the Internet

Instructions Part C.1: Locating the MAC Address on a Computer

In this part of the lab, you will determine the MAC address of a computer using the Windows ipconfig command.

Step 1: Display information for the command ipconfig / all.

a. Right-click on the Start button and select Command Prompt.

b. Enter the ipconfig /all command at the command prompt.

Step 2: Locate the MAC (physical) address(es) in the output from the ipconfig /all command.

Use the table below to fill in the description of the Ethernet adapter and the physical (MAC) Address:

Question: How many MAC addresses did you discover in your PC?

5

Part C.2: Analyzing the Parts of a MAC Address

The second part of the address, the remaining 3 bytes, are the unique ID for the interface. All MAC addresses that begin with the same OUI must have unique values in the last 3 bytes.

In this example, the physical MAC address for the Ethernet LAN interface is D4-BE-D9-13-63-00.

Step 1: List MAC addresses discovered by you and your classmates in the previous part.

List the 3-byte Manufacturer OUI and the 3-byte unique interface identifier. You will fill in the Vendor name in the table below.

Step 2: Look up the vendors who are the registered owners of the OUIs that you listed in the table.

a. Wireshark.org provides an easy-to-use lookup tool at https://www.wireshark.org/tools/ouilookup.html. Use this tool or use the Internet to search for other ways to identify an OUI.

b. Use the information that you found to update the vendor column in the chart in Step 1.

Question: How many different vendors did you discover?

2

Reflection

1. Why might a computer have more than one MAC address?

A computer can have multiple NIC which are for ethernet and wireless.

2. The sample output from the ipconfig /all command shown previously had only one MAC address. Suppose the output was from a computer that also had wireless Ethernet capability. How might the output change?

The screen will show information of all NIC enabled on the computer

3. Try connecting and disconnecting the network cable(s) to your network adapter(s) and use the ipconfig /all command again. What changes do you see? Does the MAC address still display? Will the MAC address ever change?

4. What are other names for the MAC address?

MAC address is also known as hardware address, ethernet address, or burned-in address (BIA)

## Engagement Structure 
<p>A core function of the red team is adversary emulation. While not mandatory, it is commonly used to assess what a real adversary would do in an environment using their tools and methodologies. The red team can use various cyber kill chains to summarize and assess the steps and procedures of an engagement.

The blue team commonly uses cyber kill chains to map behaviors and break down an adversaries movement. The red team can adapt this idea to map adversary TTPs (Tactics, Techniques, and Procedures) to components of an engagement.

Many regulation and standardization bodies have released their cyber kill chain. Each kill chain follows roughly the same structure, with some going more in-depth or defining objectives differently. Below is a small list of standard cyber kill chains.</p>


* [Lockheed Martin Cyber Kill Chain](https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html)
* [Unified Kill Chain](https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html)
*  [Varonis Cyber Kill Chain](https://www.varonis.com/blog/cyber-kill-chain/)
* [Active Directory Attack Cycle](https://www.varonis.com/blog/cyber-kill-chain/)
* [MITRE ATT&CK Framework](https://attack.mitre.org/) 

<h3>Components of the kill chain are broken down in the table below.</h3>
<table class="table table-bordered">
<thead>
<tr>
<th>Technique</th>
<th>Purpose</th>
<th>Examples</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left">Reconnaissance</td>
<td style="text-align:left">Obtain information on the target</td>
<td style="text-align:left"><span>Harvesting emails, <a class="Gx6hZL4g glossary-term" onclick="initPopOver('OSINT', 'Gx6hZL4g')">OSINT</a></span></td>
</tr>
<tr>
<td style="text-align:left">Weaponization</td>
<td style="text-align:left">Combine the objective with an exploit. Commonly results in a deliverable payload.</td>
<td style="text-align:left">Exploit with backdoor, malicious office document</td>
</tr>
<tr>
<td style="text-align:left">Delivery</td>
<td style="text-align:left">How will the weaponized function be delivered to the target</td>
<td style="text-align:left">Email, web, USB</td>
</tr>
<tr>
<td style="text-align:left">Exploitation</td>
<td style="text-align:left">Exploit the target's system to execute code</td>
<td style="text-align:left">MS17-010, Zero-Logon, etc.</td>
</tr>
<tr>
<td style="text-align:left">Installation</td>
<td style="text-align:left">Install malware or other tooling</td>
<td style="text-align:left">Mimikatz, Rubeus, etc.</td>
</tr>
<tr>
<td style="text-align:left">Command &amp; Control</td>
<td style="text-align:left">Control the compromised asset from a remote central controller</td>
<td style="text-align:left">Empire, Cobalt Strike, etc.</td>
</tr>
<tr>
<td style="text-align:left">Actions on Objectives</td>
<td style="text-align:left">Any end objectives: ransomware, data exfiltration, etc.</td>
<td style="text-align:left">Conti, LockBit2.0, etc.</td>
</tr>
</tbody>
</table>

<h1 align="center">

<img src="../assets/engagement-structure.png" alt="Tools" width="600">
</h1>

##  Defining Scope and Objectives
Engagements can be very complex and bureaucratic. The key to a successful engagement is clearly defined client objectives or goals. Client objectives should be discussed between the client and red team to create a mutual understanding between both parties of what is expected and provided. Set objectives are the basis for the rest of the engagement documentation and planning.

Without clear and concrete objectives and expectations, you are preparing for a very unstructured and unplanned campaign. Objectives set the tone for the rest of the engagement.

When assessing a client's objectives and planning the engagement details, you will often need to decide how focused the assessment is.



Below is an example of the client objectives of a mature organization with a strong security posture.

###  Example 1 - Global Enterprises:

<b>Objectives:</b>

<ol>
  <li>Identify system misconfigurations and network weaknesses.</li>
    <ol>
      <li>Focus on exterior systems.</li>
    </ol>
  <li>Determine the effectiveness of endpoint detection and response systems.</li>
  <li>Evaluate overall security posture and response. </li>
      <ol>
      <li>SIEM and detection measures.</li>
      <li>Remediation.</li>
      <li>Segmentation of DMZ and internal servers.</li>
    </ol>
    <li>Use of white cards is permitted depending on downtime and length.</li>
     <li>Evaluate the impact of data exposure and exfiltration.</li>
</ol> 

<b>Scope:</b>

<ol>
  <li>System downtime is not permitted under any circumstances.</li>
    <ol>
      <li>Any form of DDoS or DoS is prohibited.</li>
      <li>Use of any harmful malware is prohibited; this includes ransomware and other variations.</li>
    </ol>
  <li>Exfiltration of PII is prohibited. Use arbitrary exfiltration data.</li>
  <li>Attacks against systems within 10.0.4.0/22 are permitted.</li>
  <li>Attacks against systems within 10.0.12.0/22 are prohibited.</li>
  <li>Bean Enterprises will closely monitor interactions with the DMZ and critical/production systems. 
    <ol>
    <li>Any interaction with "*.bethechange.xyz" is prohibited.</li>
      <li>All interaction with "*.globalenterprises.thm" is permitted.</li>
  </ol>
  </li>
</ol> 

## Red Team Rules of Engagement

<p>Rules of Engagement (RoE) are a legally binding outline of the client objectives and scope with further details of engagement expectations between both parties. This is the first "official" document in the engagement planning process and requires proper authorization between the client and the red team.</p>

<p>The format and wording of the RoE are critical since it is a legally binding contract and sets clear expectations.</p>

<table class="table table-bordered"><tbody><tr><td><b>Section Name</b></td><td><b>Section Details</b></td></tr><tr><td>Executive Summary</td><td>Overarching summary of all contents and authorization within&nbsp;RoE&nbsp;document<br></td></tr><tr><td>Purpose</td><td>Defines why the&nbsp;RoE&nbsp;document is used</td></tr><tr><td>References</td><td>Any references used throughout the&nbsp;RoE&nbsp;document (HIPAA,&nbsp;ISO, etc.)<br></td></tr><tr><td>Scope</td><td>Statement of the agreement to restrictions and guidelines<br></td></tr><tr><td>Definitions</td><td>Definitions of technical terms used throughout the&nbsp;RoE&nbsp;document<br></td></tr><tr><td>Rules of Engagement and Support Agreement</td><td>Defines obligations of both parties and general technical expectations of engagement conduct<br></td></tr><tr><td>Provisions</td><td>Define exceptions and additional information from the Rules of Engagement<br></td></tr><tr><td>Requirements, Restrictions, and Authority&nbsp;</td><td>Define specific expectations of the red team cell<br></td></tr><tr><td>Ground Rules</td><td>Define limitations of the red team cell's interactions<br></td></tr><tr><td>Resolution of Issues/Points of Contact</td><td>Contains all essential personnel involved in an engagement<br></td></tr><tr><td>Authorization</td><td>Statement of authorization for the engagement<br></td></tr><tr><td>Approval&nbsp;</td><td>Signatures from both parties approving all subsections of the preceding document<br></td></tr><tr><td>Appendix</td><td>Any further information from preceding subsections<br></td></tr></tbody></table>

Example of RoE in this file [GlobalEnterprisesRoE](./GlobalEnterprisesRoE.pdf)


You can see more about RoE Template in [readteam.guide](https://redteam.guide/docs/templates/roe_template/)

## Credits

* http://tryhackme.com
* http://readteam.guide
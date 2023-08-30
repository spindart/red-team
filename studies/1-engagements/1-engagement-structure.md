## Engagement Structure

<p>A core function of the red team is adversary emulation. While not mandatory, it is commonly used to assess what a real adversary would do in an environment using their tools and methodologies. The red team can use various cyber kill chains to summarize and assess the steps and procedures of an engagement.

The blue team commonly uses cyber kill chains to map behaviors and break down an adversaries movement. The red team can adapt this idea to map adversary TTPs (Tactics, Techniques, and Procedures) to components of an engagement.

Many regulation and standardization bodies have released their cyber kill chain. Each kill chain follows roughly the same structure, with some going more in-depth or defining objectives differently. Below is a small list of standard cyber kill chains.</p>

- [Lockheed Martin Cyber Kill Chain](https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html)
- [Unified Kill Chain](https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html)
- [Varonis Cyber Kill Chain](https://www.varonis.com/blog/cyber-kill-chain/)
- [Active Directory Attack Cycle](https://www.varonis.com/blog/cyber-kill-chain/)
- [MITRE ATT&CK Framework](https://attack.mitre.org/)

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

<img src="assets/engagement-structure.png" alt="Tools" width="600">
</h1>
<br>
<a href="./2-defining-scope-and-structure.md">>> Defining Scope and Structure</a>
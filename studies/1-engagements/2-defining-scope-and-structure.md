## Defining Scope and Objectives

Engagements can be very complex and bureaucratic. The key to a successful engagement is clearly defined client objectives or goals. Client objectives should be discussed between the client and red team to create a mutual understanding between both parties of what is expected and provided. Set objectives are the basis for the rest of the engagement documentation and planning.

Without clear and concrete objectives and expectations, you are preparing for a very unstructured and unplanned campaign. Objectives set the tone for the rest of the engagement.

When assessing a client's objectives and planning the engagement details, you will often need to decide how focused the assessment is.

Below is an example of the client objectives of a mature organization with a strong security posture.

### Example 1 - Global Enterprises:

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
<br>
<a href="./3-roe.md">>> Rules of Engagement</a>
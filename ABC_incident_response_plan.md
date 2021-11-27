# Incident Response Plan

This document offers guidance for employees or incident responders who believe they have discovered or are responding to a security incident.

## Escalation

If you are a user who discovers a malware in our product, please email to it-support@abc.com.

If you are one of our IT-support staff, please use these communication channels in case of a security breach incident: send a short report via your it-support@abc.com email to the CTO@abc.com in case your analysts don´t know how to deal with the issue and the level of severity is critical.

In case you contained the issue in first line of defence please note the threat and resolvement in our #known_threats channel on Slack.

In case the threat breaches through the first line of defense and your analysts cant contain it, please communicate the issue on Slack in our #second_line_of_defence_threats.

All of our slack channels have memebers with the same scope of privilege in them. For example, the administrators will all have access to #second_line_of_defence_threats which will be available for access with a special generated password.

All entries via email require to be accessed through tor browser so that communication cannot be tracked.

Remember to be a good witness. Behave as if you were reporting a crime and include lots of specific details about what you have discovered.

Note: do not spam the CTO´s email, the company´s VLAN will filter and freeze after two or more consequtive pings from the same personal IP address.

## Severity

Here we will try to describe different levels of severity, so that it is easier to differentiate how to act on different types of incidents.

### Low and Medium Severity

Issues meeting this severity are simply suspicions or odd behaviors. They are not verified and require further investigation. There is no clear indicator that systems have tangible risk and do not require emergency response. This includes suspicious emails, outages, strange activity on a laptop.

For example, if you are an analyst in our defense team capturing the traffic via wireshark and then analysing the traffic offline; look for red and black color coded events. If any of this TCP protocols have a more serious implications like constant received encrypted traffic from unknown and unsecure IP addresses, then forward the issue to second line of defense response team for further investigation as it may be a high severity risk.

### High Severity

High severity issues relate to problems where an adversary or active exploitation hasn’t been proven yet, and may not have happened, but likely to happen. This may include vulnerabilities with direct risk of exploitation, threats with risk or adversarial persistence on our systems (eg: backdoors, malware), malicious access of business data (eg: passwords, vulnerability data, payments information), or threats that put any individual at risk of physical harm.

High severity issues should include an email to security_team@abc.com with “High severity” in the subject line, or a message to #second_line_of_defence_threats with “@channel” in the message to alert all of our incident responders.

### Critical Severity

Critical issues relate to actively exploited risks and involve a malicious actor. Identification of active exploitation is critical to this severity category.

Critical severity issues should involve a message to “@channel” in #second_line_of_defence_threats as well as messages to the CTO and COO to their emails CTO@abc.com and COO@abc.com, respectively. Put in subject line "Critical risk". Continue escalation until you receive acknowledgement. In case of identified malware CEO and PR need to be notified on their emails CEO@abc.com and PR@abc.com, respectively. Involvement of a crisis lead for public relations, a lawyer familiar with breach notification, and a “heads up” to our consultant response partners are highly recommended.

## Internal Issues

Issues where the malicious actor is an internal employee, contractor, vendor, or partner requires sensitive handling. Please contact the CEO and CTO directly and do not discuss with other employees. These are critical issues and must be pushed to follow up.

## Compromised Communications

If there are IT communication risks, the San Francisco team will announce an out of band solution within the office, and will communicate this to managers with directions over cell phones.

Incident responders must have second form of communication available at all times, such as wickr profiles.

## Response Steps

For critical issues, the response team will follow an iterative response process designed to investigate, contain exploitation, remediate our vulnerability, and document a post-mortem with the lessons of an incident.

1. CTO or CEO will determine if a lawyer be included and attorney client privilege between responders will begin.
2. A central “War Room” will be designated.
3. The following meeting will occur at regular intervals until the incident is resolved:

### Breach Response Meeting — Agenda

- Update Breach Timeline
- New Indicators of Compromise
- Investigative Q&A
- Emergency Mitigations
- Long Term Mitigations (including Root Cause Analysis)
- Everything Else

Solutions:
We will update newest info from reflections on incident onto a breach timeline within the company internal channels, with all known temporal data related to the incident. All employees and outside actors who compromised the integrity of the company will shared publicly according to the seriousness of the breach. The security teams will add new knowns and unknowns of the threats to the #known_threats channel. A list of tactical Emergency Mitigations will be updated. A list of long term, post breach Long Term Mitigations will be updated. Once items related to response are covered, technical responders may leave the meeting and meta-topics related to the breach which are discussed (communications, legal issues, blog posts, etc) with leadership.

## Response Team Members

| Name    | Cell Phones | wickr      | signal     | pgp     |
| ------- | ----------- | ---------- | ---------- | ------- |
| ember   | 60-51-52-74 | emem@wickr | em@signal  | em@pgp  |
| Viviene | 60-66-77-88 | viv@wickr  | viv@signal | em@pgp  |
| Namita  | 60-77-55-77 | nam@wickr  | nam@signal | nam@pgp |

## External Contact

| Name                | Function                      | Email                 | Phone         |
| ------------------- | ----------------------------- | --------------------- | ------------- |
| ACME Forensics      | Forensic Response             | whoa@email.com        | (777)-555-555 |
| Krisis Management   | PR Augmentation               | hey@email.com         | (777)-555-555 |
| SF FBI Field Office | Law Enforcement               | hello_world@email.com | (777)-555-555 |
| J&L Law Partners    | Breach Notification Expertise | heya@email.com        | (777)-555-555 |

## Runbooks

> If you have any specific "How To"'s for common investigations, include them here.

## Required Retrospective

> If you want this document to be focused on emergency handling only, you can strike this section.

Update reports once a week. Inform all the team members of the changes give chance to add to the lists or discuss common threats.

All incidents meeting "High" severity classification must be a part of the regularly scheduled weekly outage meeting.

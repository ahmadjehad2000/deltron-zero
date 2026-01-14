---
layout: post
title: "MARKDOWN TEST - ALL FEATURES"
date: 2026-01-14 10:00:00
---

# H1 Header - Main Title

This is a test post to showcase all markdown formatting capabilities in the Deltron Zero terminal interface.

## H2 Header - Section Title

This section demonstrates various text formatting options and content types.

### H3 Header - Subsection

Regular paragraph text with **bold text**, *italic text*, and ***bold italic text***. You can also use `inline code` within sentences.

#### H4 Header - Minor Section

Even smaller headers work great for detailed breakdowns.

##### H5 Header - Deep Dive

And we can go deeper if needed.

###### H6 Header - Maximum Depth

This is the smallest header available in markdown.

---

## Text Formatting Examples

**Bold Statement:** This text is important and draws attention.

*Italic Emphasis:* This text has subtle emphasis.

***Combined Bold and Italic:*** Maximum emphasis for critical information.

~~Strikethrough text~~ for corrections or deprecated info.

> **Blockquote Section:**
> This is a blockquote that can span multiple lines.
> Perfect for highlighting important quotes or notes.
> 
> You can even have multiple paragraphs in a blockquote.

---

## Lists and Organization

### Unordered List

- First item in the list
- Second item with some details
  - Nested item level 1
  - Another nested item
    - Even deeper nesting level 2
- Back to main level
- Final item

### Ordered List

1. First step in the process
2. Second step with explanation
3. Third step breakdown:
   1. Sub-step A
   2. Sub-step B
   3. Sub-step C
4. Fourth and final step

### Task List

- [x] Completed task
- [x] Another completed item
- [ ] Pending task
- [ ] Future work item

---

## Code Examples

### Inline Code

Use the `ls -la` command to list directory contents, or run `sudo apt update` for system updates.

### Code Block - Python
```python
# Python example - Exploit scanner
import socket
import sys

def scan_port(target, port):
    try:
        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
        sock.settimeout(1)
        result = sock.connect_ex((target, port))
        if result == 0:
            print(f"[+] Port {port} is OPEN")
        sock.close()
    except Exception as e:
        print(f"[-] Error: {e}")

# Scan common ports
target = "192.168.1.1"
for port in [21, 22, 80, 443, 3389]:
    scan_port(target, port)
```

### Code Block - Bash
```bash
#!/bin/bash
# Security audit script

echo "[*] Starting security audit..."

# Check for listening ports
echo "[+] Checking open ports:"
netstat -tuln | grep LISTEN

# Check for suspicious processes
echo "[+] Checking processes:"
ps aux | grep -E 'suspicious|malware'

# Review SSH logs
echo "[+] Recent SSH attempts:"
tail -20 /var/log/auth.log | grep ssh

echo "[*] Audit complete!"
```

### Code Block - JavaScript
```javascript
// XSS Detection example
function detectXSS(input) {
  const dangerousPatterns = [
    /<script\b[^<]*(?:(?!<\/script>)<[^<]*)*<\/script>/gi,
    /javascript:/gi,
    /on\w+\s*=/gi
  ];
  
  for (let pattern of dangerousPatterns) {
    if (pattern.test(input)) {
      console.log('[!] XSS pattern detected!');
      return true;
    }
  }
  return false;
}

// Test the function
const userInput = '<script>alert("XSS")</script>';
detectXSS(userInput);
```

---

## Tables

### Basic Table

| Protocol | Port | Status | Notes |
|----------|------|--------|-------|
| SSH | 22 | OPEN | Secure access |
| HTTP | 80 | OPEN | Web traffic |
| HTTPS | 443 | OPEN | Encrypted web |
| FTP | 21 | CLOSED | Disabled |
| RDP | 3389 | FILTERED | Firewalled |

### Aligned Table

| Tool | Purpose | Difficulty | Rating |
|:-----|:-------:|:----------:|-------:|
| Nmap | Port Scanning | Easy | ⭐⭐⭐⭐⭐ |
| Metasploit | Exploitation | Medium | ⭐⭐⭐⭐ |
| Burp Suite | Web Testing | Medium | ⭐⭐⭐⭐⭐ |
| Wireshark | Packet Analysis | Hard | ⭐⭐⭐⭐ |

---

## Links and References

### External Links

Check out these resources:
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [CWE Database](https://cwe.mitre.org/)
- [NVD Vulnerabilities](https://nvd.nist.gov/)

### Internal Navigation

See also:
- [Back to Home](/)
- [View Projects](/projects)
- [Search Archives](/search)

---

## Images

### Remote Image (From URL)

![Cybersecurity Concept](https://images.unsplash.com/photo-1550751827-4bd374c3f58b?w=800&q=80)

*Caption: Modern cybersecurity infrastructure*

### Placeholder Image

![Security Network](https://via.placeholder.com/800x400/0a0a0a/44FF44?text=SECURITY+NETWORK+DIAGRAM)

*Caption: Network topology visualization*

### Another Example

![Terminal Interface](https://via.placeholder.com/600x300/0a0a0a/FFB000?text=TERMINAL+ACCESS+GRANTED)

---

## Special Formatting

### Horizontal Rules

Use horizontal rules to separate sections:

---

***

___

### Escape Characters

Use backslash to escape special characters: \* \_ \` \# \[ \]

### HTML Elements (if supported)

<div style="padding: 15px; border: 1px solid #44FF44; margin: 20px 0;">
  <strong>ALERT:</strong> This is a custom HTML alert box.
</div>

---

## Nested Complex Example

Here's a complex nested structure:

1. **Main Security Phase**
   - Reconnaissance
     - Passive information gathering
```bash
       whois example.com
       nslookup example.com
```
     - Active scanning
```bash
       nmap -sV -sC target.com
```
   
2. **Exploitation Phase**
   > Remember: Always have written authorization before testing!
   
   - Vulnerability identification
   - Exploit selection
   - Payload delivery

3. **Post-Exploitation**
   - [ ] Establish persistence
   - [ ] Privilege escalation
   - [ ] Data exfiltration
   - [x] Cover tracks

---

## Mathematical Notation

If supported: E = mc² or x² + y² = z²

Inline formula: The complexity is O(n log n).

---

## Emoji Support 🔒

- 🔐 Security
- 🛡️ Defense
- 🔍 Investigation
- ⚠️ Warning
- ✅ Success
- ❌ Failed
- 💻 Computing
- 🌐 Network

---

## Summary

This post demonstrates:

✓ All header levels (H1-H6)  
✓ Text formatting (bold, italic, code)  
✓ Lists (ordered, unordered, nested, tasks)  
✓ Code blocks with syntax highlighting  
✓ Tables with alignment  
✓ Links (internal and external)  
✓ Images (remote URLs)  
✓ Blockquotes  
✓ Horizontal rules  
✓ Special characters  

---

**Transmission Status:** COMPLETE  
**Data Integrity:** VERIFIED  
**Classification:** PUBLIC  

`[END_TRANSMISSION]`

# interview-prep

My practice log for **QA Automation / DevOps** co-op interviews: coding problems, SQL, Bash, Go, and the core concepts behind networking, Linux, testing, DevOps and security.

Each solution is written in my own words with:
- the approach
- time and space complexity
- what I learned or got wrong the first time

---

## Repository structure

```
interview-prep/
├── README.md          # this checklist
├── leetcode/          # Python solutions, e.g. 0001_two_sum.py
├── sql/               # SQL solutions, e.g. 0175_combine_two_tables.sql
├── bash/              # Bash solutions, e.g. 0195_tenth_line.sh
├── go/                # Go basics, Go solutions and small tools
└── notes/             # concept notes
    ├── networking.md
    ├── linux-os.md
    ├── testing.md
    ├── devops.md
    └── security.md
```

---

## 1. Coding (Python)

### Arrays & Hashing
- [ ] 1. Two Sum
- [ ] 217. Contains Duplicate
- [ ] 242. Valid Anagram
- [ ] 49. Group Anagrams
- [ ] 347. Top K Frequent Elements
- [ ] 238. Product of Array Except Self

### Two Pointers
- [ ] 125. Valid Palindrome
- [ ] 11. Container With Most Water
- [ ] 15. 3Sum

### Sliding Window
- [ ] 121. Best Time to Buy and Sell Stock
- [ ] 3. Longest Substring Without Repeating Characters

### Stack
- [ ] 20. Valid Parentheses
- [ ] 155. Min Stack
- [ ] 739. Daily Temperatures

### Binary Search
- [ ] 704. Binary Search
- [ ] 33. Search in Rotated Sorted Array

### Linked List
- [ ] 206. Reverse Linked List
- [ ] 21. Merge Two Sorted Lists
- [ ] 141. Linked List Cycle

### Trees
- [ ] 104. Maximum Depth of Binary Tree
- [ ] 226. Invert Binary Tree
- [ ] 102. Binary Tree Level Order Traversal
- [ ] 98. Validate Binary Search Tree

### Graphs
- [ ] 200. Number of Islands
- [ ] 133. Clone Graph
- [ ] 207. Course Schedule

### Heap
- [ ] 215. Kth Largest Element in an Array

### Dynamic Programming
- [ ] 70. Climbing Stairs
- [ ] 198. House Robber
- [ ] 322. Coin Change

---

## 2. SQL

- [ ] 1757. Recyclable and Low Fat Products
- [ ] 175. Combine Two Tables
- [ ] 182. Duplicate Emails
- [ ] 183. Customers Who Never Order
- [ ] 181. Employees Earning More Than Their Managers
- [ ] 197. Rising Temperature
- [ ] 176. Second Highest Salary
- [ ] 184. Department Highest Salary

---

## 3. Bash

- [ ] 195. Tenth Line
- [ ] 193. Valid Phone Numbers
- [ ] 192. Word Frequency
- [ ] 194. Transpose File

---

## 4. Go

Go is the language behind Docker, Kubernetes and Terraform, so it is common in DevOps teams.

### Basics
- [ ] Install Go, `go mod init`, `go run`, `go build`
- [ ] Variables, types, `if` / `for` / `switch`
- [ ] Slices and maps
- [ ] Structs and methods
- [ ] Interfaces
- [ ] Error handling (`if err != nil`)
- [ ] Goroutines and channels
- [ ] Testing with `go test` and table-driven tests

### Re-solve in Go
- [ ] 1. Two Sum
- [ ] 20. Valid Parentheses
- [ ] 206. Reverse Linked List
- [ ] 704. Binary Search
- [ ] 200. Number of Islands

### Small tools
- [ ] CLI that reads a file and counts lines and words (uses `flag` and `os`)
- [ ] HTTP health checker: send requests to a list of URLs and report status codes and response times
- [ ] Concurrent version of the health checker using goroutines
- [ ] Tiny REST API with `net/http` that returns JSON, plus tests

---

## 5. Networking concepts → `notes/networking.md`

- [ ] OSI model vs TCP/IP model (what each layer does, one example protocol per layer)
- [ ] TCP vs UDP, and when to use each
- [ ] TCP three-way handshake and connection teardown
- [ ] What happens when you type a URL into a browser
- [ ] DNS resolution step by step
- [ ] HTTP vs HTTPS, common HTTP methods and status codes
- [ ] TLS handshake (high level)
- [ ] IP addresses, subnetting and CIDR (e.g. how many hosts in a /24)
- [ ] NAT, DHCP and ARP
- [ ] Common ports (22, 53, 80, 443, 5432 …)
- [ ] Load balancer: Layer 4 vs Layer 7
- [ ] Firewall, VPN and proxy: what each one does
- [ ] Hands-on: `ping`, `traceroute`, `dig`, `curl -v`, `ss`, Wireshark capture of a handshake

---

## 6. Linux & OS concepts → `notes/linux-os.md`

- [ ] Process vs thread
- [ ] Concurrency, race conditions, deadlock
- [ ] Stack vs heap, virtual memory
- [ ] File permissions (`chmod 755` explained), users and groups
- [ ] Signals (`SIGTERM` vs `SIGKILL`)
- [ ] Environment variables and `PATH`
- [ ] Hands-on: `grep`, `awk`, `sed`, `find`, `ps`, `top`, `kill`, `systemctl`, `journalctl`, `cron`

---

## 7. Testing / QA concepts → `notes/testing.md`

- [ ] Test pyramid: unit vs integration vs end-to-end
- [ ] Black-box vs white-box testing
- [ ] Equivalence partitioning and boundary value analysis
- [ ] Smoke vs sanity vs regression testing
- [ ] How to write a good bug report
- [ ] Mocking: what it is and when to use it
- [ ] pytest: fixtures, `parametrize`, testing exceptions
- [ ] API testing with Python `requests`
- [ ] UI automation basics (Playwright or Selenium)
- [ ] Practice: write test cases for a login page

---

## 8. DevOps concepts → `notes/devops.md`

- [ ] CI vs Continuous Delivery vs Continuous Deployment
- [ ] Docker: image vs container, layers and caching
- [ ] Kubernetes: Pod, Deployment, Service, Job
- [ ] Infrastructure as Code (Terraform `init` / `plan` / `apply`)
- [ ] Deployment strategies: rolling, blue-green, canary
- [ ] Logging vs monitoring vs alerting
- [ ] Git: merge vs rebase, branching strategies
- [ ] Secrets management (why keys never go in Git)

---

## 9. Security concepts → `notes/security.md`

- [ ] CIA triad
- [ ] Authentication vs authorization
- [ ] Hashing vs encryption, and why passwords need a salt
- [ ] Symmetric vs asymmetric encryption
- [ ] OWASP Top 10 (SQL injection, XSS, CSRF …)
- [ ] Principle of least privilege
- [ ] JWT and OAuth 2.0 (high level)
- [ ] CVE vs CVSS score
- [ ] Brute-force protection: account lockout, rate limiting

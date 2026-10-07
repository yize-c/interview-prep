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

---

## 10. SQL playground

Practice on my site's in-browser SQL playground (yize-c.github.io/learn.html#sql). Each line must match an exercise there word for word.

- [ ] 1. SELECT / FROM: Show the name and major of every student.
- [ ] 2. SELECT / FROM: Show the title and number of credits of every course.
- [ ] 3. SELECT / FROM: Show every column of the enrollments table.
- [ ] 4. WHERE: Find the names of students who live in Victoria.
- [ ] 5. WHERE: Find enrollments with a grade of 85 or higher. Show student_id, course_id, and grade.
- [ ] 6. WHERE: Find enrollments that don't have a grade yet. Show student_id and course_id.
- [ ] 7. ORDER BY: List every student's name, year, and city, with the highest year first. For students in the same year, sort by city A–Z, and then by name A–Z.
- [ ] 8. ORDER BY: List course titles and credits, from the most credits to the fewest. For courses with the same credits, sort titles A–Z.
- [ ] 9. ORDER BY: Show the 3 highest grades (student_id, course_id, grade), highest first.
- [ ] 10. COUNT / SUM: How many students are there?
- [ ] 11. COUNT / SUM: What is the total number of credits across all courses?
- [ ] 12. COUNT / SUM: How many enrollments have a grade? (Don't count the ones without a grade.)
- [ ] 13. GROUP BY: How many students are in each major? Show the major and the count.
- [ ] 14. GROUP BY: How many students are enrolled in each course? Show course_id and the count.
- [ ] 15. GROUP BY: What is the highest grade in each term? Show term and the highest grade.
- [ ] 16. LEFT JOIN: List every student's name with the course_id of each of their enrollments. Students with no enrollments must still appear, with NULL as the course_id.
- [ ] 17. LEFT JOIN: List every course title with how many enrollments it has. Courses with no enrollments should show 0.
- [ ] 18. LEFT JOIN: Find the names of students who aren't enrolled in any course.
- [ ] 19. HAVING: Which majors have more than 2 students? Show the major and the count.
- [ ] 20. HAVING: Which students are enrolled in at least 3 courses? Show student_id and the number of courses.
- [ ] 21. HAVING: Which courses have an average grade above 80? Show course_id and the average rounded to 1 decimal place.
- [ ] 22. INNER vs LEFT JOIN: Using an INNER JOIN, list each student's name with the title of each course they're enrolled in.
- [ ] 23. INNER vs LEFT JOIN: Now start from courses and LEFT JOIN to enrollments: list every course title with the student_id of each enrollment (NULL if a course has none).
- [ ] 24. INNER vs LEFT JOIN: How many rows does students INNER JOIN enrollments return, and how many does students LEFT JOIN enrollments return? Return one row with two columns: inner_rows and left_rows.
- [ ] 25. Subqueries: Using a subquery with IN, find the names of students enrolled in course 105.
- [ ] 26. Subqueries: Find enrollments whose grade is higher than the average of all grades. Show student_id, course_id, and grade.
- [ ] 27. Subqueries: Find the title of the course (or courses) with the most credits.
- [ ] 28. CASE WHEN: For each enrollment, show student_id, course_id, and a column called result: 'in progress' if there's no grade, 'pass' if the grade is 60 or more, and 'fail' otherwise.
- [ ] 29. CASE WHEN: Label each course as 'light' (fewer than 3 credits), 'normal' (exactly 3), or 'heavy' (more than 3). Show title and the label.
- [ ] 30. CASE WHEN: In one query, count how many enrollments are passing (grade 60 or more) and how many are failing (grade below 60). Return two columns: passing and failing. Enrollments without a grade count as neither.

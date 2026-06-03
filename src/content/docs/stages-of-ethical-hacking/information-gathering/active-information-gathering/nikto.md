---
title: "Nikto"
description: ">-"
---




## Installation and introduction

[Resource Link](https://github.com/sullo/nikto)

## Default scan

```bash
# HTTP
nikto -h $DOMAIN

# HTTPS
nikto -h $DOMAIN -ssl

# Use domains from file
nikto -h domains.txt
```

#### Output&#x20;

```bash
# Simple
nikto -h $DOMAIN -o output.txt

# CSV format
nikto -h $DOMAIN -o output.csv -Format csv
```

#### Integration with metasploit

```bash
nikto -h $DOMAIN -Format msf+
```

## Advanced scan

`TO BE DONE`

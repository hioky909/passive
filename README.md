# passive

Passive is a Python CLI for basic passive reconnaissance.

## Requirements

- Python 3.8+

## Usage

```bash
./passive --help
```

```text
Welcome to passive v1.0.0

OPTIONS:
    -fn         Search with full-name
    -ip         Search with ip address
    -u          Search with username
```

### Full name lookup

```bash
./passive -fn "Jean Dupont"
```

Output includes:
- First name / last name
- Address
- Phone number

### IP lookup

```bash
./passive -ip 8.8.8.8
```

Output includes:
- ISP
- City
- Latitude/Longitude

### Username lookup

```bash
./passive -u "@user01"
```

Checks at least 5 social networks:
- Facebook
- Twitter
- LinkedIn
- Instagram
- GitHub

## Results file

Each execution stores output in:
- `result.txt` for the first run
- `result2.txt`, `result3.txt`, ... if previous files already exist

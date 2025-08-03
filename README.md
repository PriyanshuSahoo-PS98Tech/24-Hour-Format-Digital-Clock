# 24-Hour Format Digital Clock

A simple and elegant digital clock application built with Python's Tkinter library that displays the current time in 24-hour format (military time) for precision and clarity.

 <div align="center"> <img src="https://github.com/PriyanshuSahoo-PS98Tech/24-Hour-Format-Digital-Clock/blob/main/output.png" alt="24-Hour Format Digital Clock" width="250"> </div>

## **Features**

- **24-Hour Time Display**: Shows current time in military/24-hour format (00:00:00 to 23:59:59)
- **Real-time Updates**: Clock updates every second automatically
- **Clean Interface**: Modern dark theme with cyan and white text
- **Lightweight**: Minimal resource usage with simple GUI
- **Cross-platform**: Runs on Windows, macOS, and Linux
- **No AM/PM Confusion**: Clear 24-hour format eliminates time ambiguity

## **Requirements**

- Python 3.x
- Tkinter (usually comes pre-installed with Python)

## **Installation**

1. **Clone or download** the project files
2. **Ensure Python is installed** on your system
3. **Verify Tkinter availability** (run `python -c "import tkinter"` to test)

## **Usage**

1. **Run the application**:
   ```bash
   python 24_hour_Format_Digital_Clock.py
   ```

2. **The clock window will open** displaying:
   - Current time in 24-hour format (HH:MM:SS)
   - Auto-updating display every second
   - Clean black background with colored text
   - Time range from 00:00:00 (midnight) to 23:59:59

3. **Close the window** to exit the application

## **File Structure**

```
📁 Digital Clock Project/
├── 24_hour_Format_Digital_Clock.py    # Main application file
├── output.png                         # Screenshot of the application
├── LICENSE                            # Project license
└── README.md                          # Project documentation
```

## **How It Works**

The application uses Python's built-in modules:

- **`tkinter`**: Creates the GUI window and labels
- **`time`**: Retrieves system time and formats it
- **`strftime("%H:%M:%S")`**: Formats time in 24-hour format (00-23 hours)

The clock updates automatically using Tkinter's `after()` method, which schedules the update function to run every 1000 milliseconds (1 second).

## **Time Format Reference**

- **00:00:00** - Midnight
- **12:00:00** - Noon
- **13:00:00** - 1:00 PM
- **18:00:00** - 6:00 PM
- **23:59:59** - 11:59:59 PM

## **Customization**

You can easily modify the appearance by changing:

- **Colors**: Modify `background` and `foreground` parameters
- **Fonts**: Change font family, size, or style in the Label configurations
- **Window size**: Add `geometry()` method to set fixed dimensions
- **Update interval**: Change the 1000ms parameter in `window.after()`
- **Time format**: Switch to other formats using different `strftime()` patterns

## **Code Example**

```python
# Key components of the clock functionality
def update_clock():
    format_24_hour = time.strftime("%H:%M:%S")
    lbl_24.config(text=format_24_hour)
    window.after(1000, update_clock)
```

## **Author**

**Priyanshu Sahoo**

- GitHub: [@PriyanshuSahoo-PS98Tech](https://github.com/PriyanshuSahoo-PS98Tech)
- Portfolio: Creating practical desktop applications with clean, efficient code

## **License**

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

*A simple yet functional 24-hour digital clock application perfect for learning GUI development with Python Tkinter and ideal for users who prefer military time format.*

 <div align="center"> <b>⭐ Star this repository if you found it useful!</b> <br><br> <b>🕐 Perfect for desktop productivity, presentations, or learning GUI programming! 🕐</b> <br><br> <b>#PS98Tech #Python #Tkinter #DigitalClock #24HourFormat #MilitaryTime #GUI #Desktop</b> </div>

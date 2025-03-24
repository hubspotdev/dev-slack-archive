# Processed Data Documentation

This directory contains processed JSON files from the Slack data export. The data has been cleaned and standardized while maintaining the original structure and content. Reference the process log for more detailed information.

## Disclaimer
HubSpot is not responsible for or accountable to the accuracy, nature, or content of the conversations recorded in these JSON files. The data represents raw exports from Slack and has been processed for organizational purposes only.

## Processing Details

### Data Standardization
- Unix timestamps have been converted to ISO format (YYYY-MM-DD HH:MM:SS)
- Field names have been standardized (e.g., "user_profile" to "poster")
- Unicode escape sequences have been converted to their corresponding characters
- HubSpot case usage has been standardized
- Emoji shortcodes in reactions (e.g., "smile", "thumbsup") have been preserved

### Removed Elements
- Channel join messages
- Edit history
- Pin information
- Empty or null values

### File Organization
Files are organized by:
1. Channel name
2. Year
3. Month
4. Date

## File Structure
```
channel_name/
└── YYYY/
    └── MM/
        └── YYYY-MM-DD.json
```

## Notes
- All emoji shortcodes in reactions have been maintained exactly as they appear in the original data
- The original message structure and content remains intact
- Files are organized chronologically for easy access 

---
// Journal Template
---
# Journal Entry {{date:YYYY-MM-DD}}

## 📝 Today's Thoughts
![[{{date:YYYY-MM}}_thoughts]]

## 🔄 Review Previous Entries
```dataview
LIST
FROM "Journal"
WHERE file.day = this.file.day
SORT file.name DESC
```

## 📊 Linked References
```dataview
LIST
FROM [[]]
WHERE contains(file.outlinks, this.file.link)
```

---
// Today's Note Template
---
# {{date:YYYY-MM-DD}} Daily Note

## ℹ️ Metadata
- Date: {{date:YYYY-MM-DD}}
- Day: {{date:dddd}}
- Week: {{date:ww}}

## 🏷️ Tags
#daily-note #{{date:YYYY-MM}}

## 🌤️ Weather
- [Weather Report](https://weather.com) <!-- Replace with your preferred weather service -->
- Temperature: 
- Conditions: 

## 📅 Monthly Overview
![[{{date:YYYY-MM}}]]

## 🔗 Quick Links
- [[{{date:YYYY-MM}} Monthly Review]]
- [[Tasks]]
- [[Journal]]

---
// Book Review Template
---
# 📚 Book Review: {{title}}

## 📖 Book Information
- Title: 
- Author: 
- ISBN: 
- Published: 
- Pages: 
- Genre: #book #{{genre}}

## 🔗 External Links
- [Goodreads](https://www.goodreads.com/search?q={{title}})
- [Amazon](https://www.amazon.com/s?k={{title}})
- [Publisher's Website]()

## 📝 Review
### Summary


### Key Takeaways
1. 
2. 
3. 

### Favorite Quotes
> 

### Rating
⭐️ /5

## 🤔 Related Books
```dataview
LIST
FROM #book
WHERE contains(genre, this.genre)
```content://com.anthropic.claude.provider/tmp_artifact/tmp_artifact/obsidian-templates.txt
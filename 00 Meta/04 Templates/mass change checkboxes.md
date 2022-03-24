<%*
const slrvbCheckboxes = [[
"Unchecked",
"Regular", 
"Checked", 
"Dropped", 
"Forward", 
"Defer", 
"Question", 
"Half Done", 
"Add", 
"Research", 
"Important", 
"Idea", 
"Brainstorm", 
"Pro", 
"Con", 
"Quote", 
"Note", 
"Bookmark", 
"Information"
], [
" ",
"x", 
"X", 
"-", 
">", 
"D", 
"?", 
"/", 
"+", 
"R", 
"!", 
"i", 
"B", 
"P", 
"C", 
"Q", 
"N", 
"b", 
"I"
]];

const sanctumCheckboxes = [[
"Unchecked",
"Star",
"Alarm / Reminder / Notification",
"Favourite",
"Savings / Piggy bank",
"Savings alternative / Piggy bank",
"Cancelled",
"Rescheduled / Forwarded",
"Scheduled",
"Location",
"Bug / Debug",
"Failure",
"Note / Annotation",
"Pros",
"Cons",
"Win / Success / Reward",
"Bookmark / References",
"Idea / Tip",
"Important / Attention",
"Question / Cue",
"Info"
], [
" ",
"⭐",
"a",
"❤",
"s",
"S",
"-",
">",
"<",
"l",
"B",
"X",
"n",
"p",
"c",
"W",
"b",
"I",
"!",
"?",
"i"
]];

const selection = tp.file.selection();
const checkboxType = sanctumCheckboxes; //Change this
const check = await tp.system.suggester(checkboxType[0], checkboxType[1], true);

//Check Replacement
if (selection) {
    const replace = selection.split("\n").map(select => {
    if (select.match(/- \[.\]/)) {
        select = select.replace(/\[.\]/, `[${check}]`);
    }
    return select;
    }).join("\n");
    tR += replace;
} else {
    new Notice("Text must be selected");
};

%>
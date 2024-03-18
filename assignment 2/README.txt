I feel like my logic in this program is very simple but I'll do my best to explain it out.

Taking each prompt, I used either includes or startsWith and set the qualifier to etiher true or false. Setting to false allowed me to check for a negative result which was required for the one word title case. There was no other way to check if each string didn't have a space and therefore wasn't a one word title. The same logic goes for if titles started with certain articles. I needed to check that they didn't start with said articles so I used the false boolean to filter those out.

Originally, I had the other two cases verified with "=== true" at the end of the condition but truly that's redudant and wastes space and costs more money in the end. So, I deleted those additions.

I think I've explained this to the most exhaustive sense that I possibly can. To me, it's very straight-forward.
| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Title

**MakeoverMonday 2023 W16: Redesigning "Retirement Ages Around the World"**

## Step one: the visualization
I chose this dataset for a few reasons. First, I've personally been very interested in retirement age as a topic. Second, I previously worked on building a dashboard using a similar map-based format at a company I worked for, so this dataset felt familiar and relevant. Third, the original visualization was map-based and didn't show exact numbers directly on the chart, which meant readers had to constantly cross-reference the legend to figure out precise values — I saw this as a clear opportunity for improvement, since a more precise, comparison-friendly chart type could communicate the data far more effectively. Finally, the map format also collapsed the data into six broad color categories, which hid meaningful differences between countries and made the dataset a good candidate to practice a more precise redesign approach on.

2023/W16: Retirement Ages Around the World
https://makeovermonday.vercel.app/dataset/2023w16 
<img width="1200" height="1200" alt="image" src="https://github.com/user-attachments/assets/c912e80f-dcaa-43ed-9359-df607fc953e1" />

## Step two: the critique
The most immediately striking element was the illustration of an elderly couple placed on the left side of the graphic, which intuitively signals that this is data about retirement age before the reader even looks at the map. The color gradient applied to the map was also effective at conveying regional patterns at a glance, letting the reader quickly see broad geographic differences in retirement age across Europe.

On the other hand, several aspects did not work as well. First, for readers who are not familiar with European geography, the map does not clearly indicate which specific countries are being shown, making the information feel incomplete without prior geographic knowledge. Second, since the actual age values are not labeled directly on the map, readers have to repeatedly glance back and forth between the map and the legend to determine each country's exact value, which adds unnecessary friction to reading the data. Third, the six discrete color categories (60 through 65) flatten what is actually continuous data, meaning two countries with meaningfully different ages, such as 62.4 and 62.9, could be grouped into the same color and appear identical when they are not. Fourth, the visualization only shows the effective labor market exit age, while the accompanying article's central argument is about the gap between this effective age and each country's legal retirement age. Since that comparison never appears on the map itself, the visualization leaves out the very context that gives the data its meaning. Fifth, the values shown are averages of male and female data combined, which conceals the gender gap in retirement timing that exists in most countries and could be an important piece of information for this topic. Finally, while the map format is effective for an intuitive first impression, a bar chart would likely have been more effective for actually interpreting the data and grasping the precise, ranked differences between countries.

Usefulness — 8
The visualization succeeds at its core purpose: showing which countries have earlier or later effective retirement ages, and the color-coded regional breakdown clearly conveys the intended message.

Completeness — 6
The title specifies "effective" age, but the visualization never explains what makes it "effective" (i.e., how it differs from legal retirement age), leaving readers without that context. It also doesn't clarify how averages with decimal values were rounded into the six discrete categories.

Perceptibility — 6
The map format is intuitive for a first glance, but a bar chart with age values labeled directly would be far more effective for actually interpreting the data. Since country names and exact values aren't shown on the map itself, readers must constantly reference back and forth between the map and the legend.

Truthfulness — 4
As noted above, the "effective" framing in the title is never substantiated in the data itself. Retirement age is also known to vary by gender, but this visualization collapses male and female data into a single population average, obscuring that variation and limiting how accurately it represents the underlying reality.

Intuitiveness — 8
The visualization is easy to grasp at first glance: the elderly illustration immediately signals that the topic concerns older adults, and the map format immediately signals that the data is broken down by region.

Aesthetics — 8
The gradient color scheme is clean and visually pleasing, though the large illustration of the elderly couple placed next to the map feels somewhat out of place in scale and positioning; adjusting its size and placement could improve the overall composition.

Engagement — 4
The data is limited to a single metric (retirement age), which doesn't give readers much to explore further or spark deeper curiosity, the information itself feels too narrow to sustain engagement beyond the initial glance.

## Step three: Sketch a solution
<img width="2420" height="2090" alt="image" src="https://github.com/user-attachments/assets/7384f907-ab5d-4840-a522-4a3e902072ee" />

## Step four: Test the solution

**Questions to ask:**
- What elements have captured your attention?

- What area can be improved for better visual representation?

**Results:**

- Question: What elements have captured your attention?

Interviewee 1: The color contrast of blue and red

Interviewee 2: The bold and big title captured my attention

Interviewee 3: The data points of the age and plus/minus signs automatically catch my eye

- Question: What area can be improved for better visual representation?

Interviewee 1: Don't use the blue and red colors because Americans tend to intuitvely think that as politically related colors.

Interviewee 2: It would be nice to reverse the order of the data so that people can see what is ascending and descending by country.

Interviewee 3: There should be a gap between overlapping values. 


**Synthesis:**

A common pattern across the feedback I received is that the gap label is calculated relative to the effective age rather than the legal retirement age. When a chart shows "+7," viewers naturally assume this means someone worked 7 years longer than the legal retirement age, when in fact it means the opposite: the effective exit age is 7 years earlier than the legal age. This mismatch between the intuitive reading and the actual calculation baseline can seriously mislead the audience. To fix this, the gap should be explicitly anchored to the legal retirement age as the reference point, so it clearly reads as "how many years earlier people actually retire compared to the legal age." I also want to sort the data in descending order by gap size so the largest discrepancies are immediately visible at the top. 

Separately, I noticed that the subtitle in my current design is colored blue, which is the same color used for the "Legal retirement age" legend dot. This creates a visual conflict where the subtitle could be mistaken for part of the legend or for data itself. To resolve this, the subtitle color should be changed to gray, or alternatively kept in italics, so it's clearly distinguished from the chart's data elements.

## Step five: build the solution

**Final Solution**
1. What I wanted to fix first: the original only showed the "effective" age, with no comparison point

The original visualization only displayed the effective retirement age on the map, with no information about why that number was labeled "effective" or what it should be compared against. The title used the word "effective," but the legal retirement age it was implicitly being compared to was never shown anywhere.

So I added a Legal Retirement Age legend, which didn't exist in the original. My goal was to let viewers immediately grasp the insight that "this is the legal retirement age, and people are actually retiring a certain number of years earlier or later than that."

**2. Feedback I addressed first: color and the +/- baseline**
The first pieces of feedback I focused on were the color scheme and the baseline for the +/- calculation.

Color: I received feedback that, for an American audience, the red/blue color combination could be read as politically coded. To address this, I changed Legal Retirement Age to black and Effective Exit Age to blue.
Direction indicators: I also tried to use arrows to show whether the effective age was earlier (+) or later (-) than the legal age, and by how much. However, since I'm still not very familiar with Tableau, the last two countries (Estonia and Latvia) — which actually retire later than the legal age (a "-" case) — ended up with arrows pointing in the wrong direction. I intended to fix this but wasn't able to before submitting, so I'm noting it here as a known limitation.
Sorting: I also sorted the data in descending order by gap size, addressing feedback that the original ordering could be confusing to read.

**3. Other improvements**
Title: I made the title more specific so that the audience can immediately understand what the chart is comparing, clearer than in my earlier draft.
Subtitle: I removed the blue color from the subtitle, since it could be mistaken for being related to the blue legend item (Effective Exit Age).

**4. Limitations and takeaways**
Since I'm still new to Tableau's dual-axis and shape-mapping features, some issues — like the arrow direction error — remain unresolved. With more time, I would have gone back to the calculated field and fixed it.
That said, I believe the color contrast, +/- labels, and the addition of a legal-age baseline made the core message — the gap between legal and effective retirement age — much clearer than in the original.

<img width="1054" height="459" alt="Screenshot 2026-09-17 at 5 04 46 PM" src="https://github.com/user-attachments/assets/25bf985b-4c63-4d35-af71-435c70132812" />


## References
10 examples of interactive map data visualizations(Tableau): https://www.tableau.com/learn/articles/interactive-map-and-data-visualization-examples 

## AI acknowledgements
I used Claude throughout this assignment in the following ways

Tableau step-by-step guidance: Since I am still relatively new to Tableau, I used Claude to walk me through the technical steps of building the dumbbell/connected-dot chart — including pivoting the Legal Retirement Age and Effective Exit Age columns, creating calculated fields etc.


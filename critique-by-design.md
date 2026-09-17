| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Title
Text here...

_For each step below, you should document your progress as you move forward.  In terms of tone, think of the writeup as though you're keeping journal of your step-by-step process.   You should include a any insights you gained from the critique method, and what it led you to think about when considering the redesign.  You should talk about how you moved next to the sketches, and any insights you gleaned from your user feedback.  Document what you changed based on the user feedback in your redesign.  Finally, talk about what your redesigned data visualization shows, why you selected the data visualization you did, and what you attempted to show or do differently._

_You can include screenshots, sketches or other artifacts with your narrative to help tell the story of how you moved through the process.  Again, make sure to avoid including any personally identifying information about your interviewees (don't list full names, etc.).  While this template serves as a guide, make sure to reference the assignment writeup on Canvas for the official guidance.  This template does not include all guidance mentioned on the assignment page._

## Step one: the visualization

2023/W16: Retirement Ages Around the World
https://makeovermonday.vercel.app/dataset/2023w16 
<img width="1200" height="1200" alt="image" src="https://github.com/user-attachments/assets/c912e80f-dcaa-43ed-9359-df607fc953e1" />

## Step two: the critique
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
The gradient color scheme is clean and visually pleasing, though the large illustration of the elderly couple placed next to the map feels somewhat out of place in scale and positioning, adjusting its size and placement could improve the overall composition.

Engagement — 4
The data is limited to a single metric (retirement age), which doesn't give readers much to explore further or spark deeper curiosity, the information itself feels too narrow to sustain engagement beyond the initial glance.

## Step three: Sketch a solution
<img width="2420" height="2090" alt="image" src="https://github.com/user-attachments/assets/7384f907-ab5d-4840-a522-4a3e902072ee" />

## Step four: Test the solution

_Before you conduct your interviews, prepare a simple script.  Use this as a guide and as a way to take notes as you go forward. Come up with your own list of questions you want to ask for the selected visualization. Keep the questions broad so you can get the most value out of your feedback. Then, document answers to your questions here._

Questions to ask (modify these for your own interviews): 

- Can you tell me what you think this is?

- Can you describe to me what this is telling you?

- Is there anything you find surprising or confusing?

- Who do you think is the intended audience for this?

- Is there anything you would change or do differently?

Results: 

_Don't identify or share personally identifiable information (PII) about the people you spoke to._

- Question: What elements have captured your attention?

Interviewee 1: The color contrast of blue and red

Interviewee 2: The bold and big title captured my attention

Interviewee 3: The data points of the age and plus/minus signs automatically catch my eye

- Question: What area can be improved for better visual representation?

Interviewee 1: Don't use the blue and red colors because Americans tend to intuitvely think that as politically related colors.

Interviewee 2: It would be nice to reverse the order of the data so that people can see what is ascending and descending by country.

Interviewee 3: There should be a gap between overlapping values. 


Synthesis: 

_What patterns in the feedback emerge?  What did you learn from the feedback?  Based on this feedback, come up with what design changes you think might make the most sense in your final redesign._

A common pattern across the feedback I received is that the gap label is calculated relative to the effective age rather than the legal retirement age. When a chart shows "+7," viewers naturally assume this means someone worked 7 years longer than the legal retirement age, when in fact it means the opposite: the effective exit age is 7 years earlier than the legal age. This mismatch between the intuitive reading and the actual calculation baseline can seriously mislead the audience. To fix this, the gap should be explicitly anchored to the legal retirement age as the reference point, so it clearly reads as "how many years earlier people actually retire compared to the legal age." I also want to sort the data in descending order by gap size so the largest discrepancies are immediately visible at the top. 

Separately, I noticed that the subtitle in my current design is colored blue, which is the same color used for the "Legal retirement age" legend dot. This creates a visual conflict where the subtitle could be mistaken for part of the legend or for data itself. To resolve this, the subtitle color should be changed to gray, or alternatively kept in italics, so it's clearly distinguished from the chart's data elements.

## Step five: build the solution

_Include and describe your final solution here. It's also a good idea to summarize your thoughts on the process overall. When you're done with the assignment, this page should all the items mentioned in the assignment page on Canvas(a link or screenshot of the original data visualization, documentation explaining your process, a summary of your wireframes and user feedback, your final, redesigned data visualization, etc.)._

## References
_List any references you used here._

## AI acknowledgements
_If you used AI to help you complete this assignment (within the parameters of the instruction and course guidelines), detail your use of AI for this assignment here._


# CSP Unit 5 – Data: Vocabulary & Concepts

## How to read this

Each lesson lists only what's new: formal vocabulary and the concepts students should walk away with. Timing, prep, links, teaching tips, and teacher dialogue are cut.

- **Vocabulary** is copied word for word from the lesson's formal vocabulary box. Lessons without a box say "No formal vocabulary" and get concepts only.
- **Good to know** terms are defined in passing in the lesson but aren't in a formal vocabulary box. Their basic definitions are my own wording.
- **Key concepts** are condensed from the lesson's overview, objectives, presenter notes, discussion goals, and Check for Understanding.

Source: Code.org CS Principles (2025–26), Unit 5 lesson plans, licensed CC BY-NC-SA 4.0. Changes made: content condensed, reorganized, and paraphrased; teacher-facing material removed.

## Lesson 1: Learning from Data

**Vocabulary**

| Term | Definition |
| --- | --- |
| Information | the collection of facts and patterns extracted from data |
| Metadata | data about data |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Causation | When one thing actually causes another to happen |

**Key concepts**

- Data visualizations help people see a lot of data at once, find patterns that would otherwise be invisible, answer questions, and generate new ones.
- A data story separates two things: what the data shows (the facts) and why that might be the case (an informed opinion).
- Correlation (formal vocabulary in Lesson 4) does not equal causation. A pattern can have many possible causes, and understanding it usually takes more research with several datasets.
- Conclusions from a chart come with uncertainty. You may not know how the data was collected, and the data shows what happened but not why.
- Metadata (where data came from, when it was collected, how much there is) helps you understand, trust, and organize a dataset. Any digital data can have metadata, such as a photo's creation date and resolution. App Lab datasets show metadata in the data tab.

## Lesson 2: Exploring One Column

**Vocabulary:** No formal vocabulary.

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Bar Chart | A chart with one bar per unique value, showing how often each value appears |
| Histogram | A chart that groups numeric values into ranges (buckets) and shows how many values fall in each range |
| Bucket Size | The width of each range in a histogram |
| Data Analysis Process | A repeated framework for working with data, covered on the lesson slides |

**Key concepts**

- Organized data (like a table or spreadsheet) makes it possible to find trends and patterns, and visualizations help reveal them.
- A chart can only answer certain questions. Part of reading a chart is deciding which questions it can and can't answer.
- Bar charts are good at showing how common each value in a column is. They become useless when a column has too many unique values.
- Histograms fix that for numeric columns by grouping values into buckets. The result has fewer, wider bars in sorted order, which is easier to read. Choosing a good bucket size matters.
- The Data Analysis Process is introduced as a framework for the whole unit. Its steps include choosing data, cleaning and processing it, visualizing it to find patterns, and drawing careful conclusions.

## Lesson 3: Filtering and Cleaning Data

**Vocabulary**

| Term | Definition |
| --- | --- |
| Cleaning Data | a process that makes the data uniform without changing its meaning (e.g., replacing all equivalent abbreviations, spellings, and capitalizations with the same word). |
| Data Filtering | choosing a smaller subset of a data set to use for analysis, for example by eliminating / keeping only certain rows in a table |

**Key concepts**

- Data needs cleaning when it's incomplete, invalid, or combined from multiple tables.
- Messy data comes from mixed formats ("two" vs. 2), different abbreviations ("February," "Feb," "Febr"), different spellings ("color," "colour"), and inconsistent capitalization ("spring," "Spring").
- The goal of cleaning is to make data uniform without changing its meaning. Uncleaned data charts the same value as different values (4 and "four").
- Datasets in App Lab's library are already cleaned. Data you create or upload yourself may not be.
- Filtering lets you look at a subset of the data without deleting rows or making new tables. Tools like the Data Visualizer filter built in.
- The hardest part of filtering is choosing what to filter by: what do all the rows you want to keep have in common?
- Cleaning and filtering are part of the Data Analysis Process. Even with filtered data, keep separating what the data shows from why it might be that way.

## Lesson 4: Exploring Two Columns

**Vocabulary**

| Term | Definition |
| --- | --- |
| Correlation | a relationship between two pieces of data, typically referring to the amount that one varies in relation to the other. |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Crosstab Chart | A chart that counts how often each combination of values from two columns appears |
| Scatter Chart | A chart that plots one point per row using two numeric columns, to show whether they're related |

**Key concepts**

- Many questions need two pieces of information (for example, time of day and happiness), so they require analyzing two columns together.
- Crosstab charts show patterns between two columns. If either column has too many values, the chart gets enormous.
- Scatter charts show whether two numeric columns follow a trend. A trend still doesn't prove causation.
- Bar charts and histograms answer questions about one column. Crosstab and scatter charts answer questions about how two columns relate.
- Choose the type of chart based on the question and the kind of data in each column.

## Lesson 5: Big, Open, and Crowdsourced Data

**Vocabulary**

| Term | Definition |
| --- | --- |
| Citizen Science | scientific research conducted in whole or part by distributed individuals, many of whom may not be scientists, who contribute relevant data to research using their own computing devices. |
| Crowdsourcing | the practice of obtaining input or information from a large number of people via the Internet |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Big Data | Datasets so large they need special tools, such as parallel and scalable systems, to store and process |
| Open Data | Data that's made freely available for anyone to use and share |

**Key concepts**

- Students jigsaw three topics (big data, crowdsourcing, and open data), then share what each is, its key vocabulary, how it uses or changes the Data Analysis Process, and what problems it's being used to solve.
- Data is being used in new ways that affect people's lives, and the Data Analysis Process looks different (or gets manipulated) depending on the context.
- Very large datasets may need parallel and scalable systems to process.
- Open data and crowdsourcing widen who can contribute to and benefit from data, as in citizen science.

## Lesson 6: Machine Learning

**Vocabulary**

| Term | Definition |
| --- | --- |
| Data Bias | data that does not accurately reflect the full population or phenomenon being studied |
| Information | the collection of facts and patterns extracted from data |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Machine Learning | When a computer recognizes patterns and makes decisions without being explicitly programmed |
| Training Data | The labeled examples used to teach a machine learning model |

**Key concepts**

- Labeling examples (like "fish" or "not fish") is a form of programming the computer. Those examples are the training data.
- A model learns patterns from its training data and uses them to label new data. Its results depend entirely on how it was trained.
- Subjective labels (like "angry" or "fun" fish) mean the model learns the trainer's opinions and biases.
- Biased data leads to incorrect or unfair conclusions. More data doesn't remove bias. Diverse training sets help address it.
- Computing innovations can reflect existing human bias through biased algorithms or biased data. Machine learning and data mining have driven advances in medicine, business, and science, but have also been used to discriminate against groups.
- Programmers should actively work to reduce bias, which can enter at any stage of software development.
- Some steps of the process need human judgment. It's worth asking which steps should or shouldn't be automated.

## Lesson 7: Algorithmic Bias

**Vocabulary**

| Term | Definition |
| --- | --- |
| Data Bias | data that does not accurately reflect the full population or phenomenon being studied |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Algorithmic Bias | When an algorithm produces unfair or skewed results for certain groups, often because of biased training data or design choices |

**Key concepts**

- People crop photos for different reasons, so no single cropping approach fits everyone.
- Training data reflects the people who create it. Data gathered from one group, such as a class of teenagers, can carry that group's biases.
- In the real-world case, Twitter's image-cropping algorithm favored lighter faces. The model learned from saliency datasets built on photo libraries that didn't represent the whole population.
- The machine isn't "racist" on its own. The bias comes from the algorithm humans built and the data they trained it on.
- Some tasks shouldn't be fully handed to an algorithm. Students practice recognizing bias, suggesting ways to reduce it, and judging a company's response to evidence of bias.
- Algorithmic bias can cause unintended harmful effects.

## Lesson 8: Project – Tell a Data Story

**Vocabulary:** No formal vocabulary. This is a two-day unit project.

**Key concepts**

- Students use the Data Analysis Process to tell a data story: choose a dataset, create an effective visualization, and describe the new insight or decision it supports.
- Choosing a dataset and creating a visualization is cyclical. Explore datasets in the Data Visualizer before committing, and look for visualizations that lead to a compelling story.
- The story should keep separating what the data shows from why that might be.

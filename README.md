# Similarweb Data Unofficial API Documentation

## Where to Find
This api can be located on [apify](https://apify.com/pintostudio/similarweb-scraper-v2)
## Overview

The Similarweb Data Actor is a powerful tool that fetches comprehensive website analytics and traffic data from Similarweb for any domain. With just a URL, you can access detailed insights about website performance, visitor demographics, traffic sources, competitors, and much more.



## What Does This Actor Do?

This actor retrieves extensive analytics data for any website, including:

- **Traffic Statistics**: Monthly visits, page views, bounce rate, time on site
- **Global & Country Rankings**: See how a website ranks globally and in specific countries
- **Geographic Distribution**: Top countries visiting the website with percentage breakdowns
- **Traffic Sources**: Direct, search, social media, referrals, and paid traffic distribution
- **Top Keywords**: Most popular search terms driving traffic to the site
- **Engagement Metrics**: Pages per visit, average session duration, bounce rates
- **AI Chatbot Traffic**: Traffic distribution from AI assistants like ChatGPT, Claude, Perplexity, etc.
- **Competitor Analysis**: Similar websites and competitors
- **Category Rankings**: Position within industry categories
- **Historical Trends**: Traffic changes over recent months

## Getting Started

### Prerequisites

- An Apify account (free or paid)
- A URL of the website you want to analyze

### Input

The actor requires only **one simple input**:

| Field | Type | Required | Description | Example |
|-------|------|----------|-------------|---------|
| `url` | String | Yes | The full URL of the website you want to analyze | `https://www.google.com/` |

**Important Notes:**
- You only need to provide the URL - the actor automatically extracts the domain
- Works with any valid URL format (the domain is extracted automatically)
- HTTPS or HTTP - both work fine

### Example Input

```json
{
  "url": "https://www.google.com/"
}
```

## How to Use

### Step 1: Access the Actor
1. Log into your Apify account
2. Navigate to this actor
3. Click "Try for free" or "Start"

### Step 2: Enter the URL
1. In the input field labeled "URL of the page", enter the website URL you want to analyze
2. Example: `https://www.amazon.com/`

### Step 3: Run the Actor
1. Click the "Start" button
2. Wait for the actor to complete (usually takes a few seconds)

### Step 4: Access Your Results
Results are available in two formats:

**1. Dataset (Recommended for most users)**
- Click on the "Dataset" tab
- View or download the data in JSON, CSV, Excel, or other formats
- Perfect for analysis and further processing

**2. Key-Value Store**
- Find the complete results saved under the key `data`
- Includes a completion timestamp
- Useful for programmatic access

## Full Json Response Example

```json
{
	"SiteName": "google.com",
	"Description": "Learn about the Certified Publisher Program. Our publishing software experts will help you maximize revenue and grow your business.",
	"TopCountryShares": [
		{
			"country": "United States of America",
			"countryCode": "US",
			"countryFlag": "https://purecatamphetamine.github.io/country-flag-icons/3x2/US.svg",
			"Value": 0.24590223044328374,
			"valueinPercentage": "24.59"
		},
		{
			"country": "India",
			"countryCode": "IN",
			"countryFlag": "https://purecatamphetamine.github.io/country-flag-icons/3x2/IN.svg",
			"Value": 0.055533909085140276,
			"valueinPercentage": "5.55"
		},
		{
			"country": "Japan",
			"countryCode": "JP",
			"countryFlag": "https://purecatamphetamine.github.io/country-flag-icons/3x2/JP.svg",
			"Value": 0.05474343423187957,
			"valueinPercentage": "5.47"
		},
		{
			"country": "Brazil",
			"countryCode": "BR",
			"countryFlag": "https://purecatamphetamine.github.io/country-flag-icons/3x2/BR.svg",
			"Value": 0.04801373747203322,
			"valueinPercentage": "4.80"
		},
		{
			"country": "United Kingdom of Great Britain and Northern Ireland",
			"countryCode": "GB",
			"countryFlag": "https://purecatamphetamine.github.io/country-flag-icons/3x2/GB.svg",
			"Value": 0.036587049425971234,
			"valueinPercentage": "3.66"
		}
	],
	"Title": "Google",
	"Engagments": {
		"BounceRate": "0.28358483196353707",
		"Month": "1",
		"Year": "2026",
		"PagePerVisit": "8.516282675924494",
		"Visits": "85756574615",
		"TimeOnSite": "610.4100441975721"
	},
	"EstimatedMonthlyVisits": [
		{
			"date": "2025-11-01",
			"visits": 82284033110,
			"percentageChange": null
		},
		{
			"date": "2025-12-01",
			"visits": 84172772881,
			"percentageChange": 2.3
		},
		{
			"date": "2026-01-01",
			"visits": 85756574615,
			"percentageChange": 1.88
		}
	],
	"GlobalRank": {
		"Rank": 1
	},
	"CountryRank": {
		"Country": 840,
		"CountryCode": "US",
		"Rank": 1
	},
	"CategoryRank": {
		"Rank": "1",
		"Category": "Computers_Electronics_and_Technology/Search_Engines"
	},
	"GlobalCategoryRank": null,
	"IsSmall": false,
	"Policy": 0,
	"TrafficSources": {
		"Social": 0.007599429014334454,
		"Paid Referrals": 0.0032674643515027855,
		"Mail": 0.002836815536330618,
		"Referrals": 0.044567463100973995,
		"Search": 0.0834589033073366,
		"Direct": 0.8582699246895208
	},
	"Category": "computers_electronics_and_technology/search_engines",
	"LargeScreenshot": "https://site-images.similarcdn.com/image?url=google.com&t=1&s=1&h=eb35e0fbafa3eb290132ffdfe47187d950d68daaa659ec1bd4b4e834b8f16461",
	"IsDataFromGa": false,
	"Countries": [
		{
			"Code": "AF",
			"UrlCode": "afghanistan",
			"Name": "Afghanistan"
		},
		{
			"Code": "AX",
			"UrlCode": "land-islands",
			"Name": "Åland Islands"
		}
		
	],
	"Competitors": {
		"TopSimilarityCompetitors": []
	},
	"Notification": {
		"Content": null
	},
	"TopKeywords": [
		{
			"Name": "gemini",
			"EstimatedValue": 99282440,
			"Volume": 100378910,
			"Cpc": 0.42
		},
		{
			"Name": "gmail",
			"EstimatedValue": 95585130,
			"Volume": 120497090,
			"Cpc": 1.74
		},
		{
			"Name": "google maps",
			"EstimatedValue": 66657600,
			"Volume": 63966790,
			"Cpc": 0.41
		},
		{
			"Name": "maps",
			"EstimatedValue": 43016910,
			"Volume": 45663980,
			"Cpc": 0.37
		},
		{
			"Name": "google",
			"EstimatedValue": 36342950,
			"Volume": 35444950,
			"Cpc": 1.32
		}
	],
	"AiTrafficDetails": {
		"Traffic": {
			"Split": [
				{
					"Name": "chatgpt.com",
					"Rank": 1,
					"Icon": "/image?url=chatgpt.com&t=2&s=1&h=a31616ae3cdef12fcfc664127563e6092e7531e7b4c3cde7e0c8c5fd3310dfc0"
				},
				{
					"Name": "perplexity.ai",
					"Rank": 2,
					"Icon": "/image?url=perplexity.ai&t=2&s=1&h=f48fa93e79e65eef47bff5b62e7037bccffb0629aecaed2d0c9f2fb25f177362"
				},
				{
					"Name": "claude.ai",
					"Rank": 3,
					"Icon": "/image?url=claude.ai&t=2&s=1&h=a3b3778e02952b653132fb6d019ed0361cff7850429377787fbdc4c86ce1565e"
				},
				{
					"Name": "chat.deepseek.com",
					"Rank": 4,
					"Icon": "/image?url=chat.deepseek.com&t=2&s=1&h=3932bcfb7ad820bd114ee43a2dba828a589d2ff19b6dc54400e0d39b2d65d377"
				},
				{
					"Name": "copilot.microsoft.com",
					"Rank": 5,
					"Icon": "/image?url=copilot.microsoft.com&t=2&s=1&h=eb2c5d699c15f4d7ff035602d8165b847ac5e2883d42a9d8eae54163cd4b47cb"
				},
				{
					"Name": "grok.com",
					"Rank": 6,
					"Icon": "/image?url=grok.com&t=2&s=1&h=5f2be8fd5c0911d0646a313793511a5a9acc4816f25a1b301774b501e7aa7c94"
				}
			],
			"Distribution": {
				"Boundary": "<500M",
				"Chart": [
					{
						"Name": "chatgpt.com",
						"Icon": "/image?url=chatgpt.com&t=2&s=1&h=a31616ae3cdef12fcfc664127563e6092e7531e7b4c3cde7e0c8c5fd3310dfc0",
						"History": [
							{
								"Date": "2026-01-01",
								"Value": 59.82779097191507
							},
							{
								"Date": "2025-12-01",
								"Value": 62.41118914555681
							},
							{
								"Date": "2025-11-01",
								"Value": 70.32488894957885
							}
						]
					},
					{
						"Name": "perplexity.ai",
						"Icon": "/image?url=perplexity.ai&t=2&s=1&h=f48fa93e79e65eef47bff5b62e7037bccffb0629aecaed2d0c9f2fb25f177362",
						"History": [
							{
								"Date": "2026-01-01",
								"Value": 19.4349856488379
							},
							{
								"Date": "2025-12-01",
								"Value": 18.758644836870157
							},
							{
								"Date": "2025-11-01",
								"Value": 7.082723888270969
							}
						]
					},
					{
						"Name": "claude.ai",
						"Icon": "/image?url=claude.ai&t=2&s=1&h=a3b3778e02952b653132fb6d019ed0361cff7850429377787fbdc4c86ce1565e",
						"History": [
							{
								"Date": "2026-01-01",
								"Value": 18.573293908514493
							},
							{
								"Date": "2025-12-01",
								"Value": 14.670453099486702
							},
							{
								"Date": "2025-11-01",
								"Value": 12.91577719623936
							}
						]
					}
				],
				"Chatbots": [
					{
						"Name": "chatgpt.com",
						"Icon": "/image?url=chatgpt.com&t=2&s=1&h=a31616ae3cdef12fcfc664127563e6092e7531e7b4c3cde7e0c8c5fd3310dfc0",
						"Value": 59.82779097191507
					},
					{
						"Name": "perplexity.ai",
						"Icon": "/image?url=perplexity.ai&t=2&s=1&h=f48fa93e79e65eef47bff5b62e7037bccffb0629aecaed2d0c9f2fb25f177362",
						"Value": 19.4349856488379
					},
					{
						"Name": "claude.ai",
						"Icon": "/image?url=claude.ai&t=2&s=1&h=a3b3778e02952b653132fb6d019ed0361cff7850429377787fbdc4c86ce1565e",
						"Value": 18.573293908514493
					}
				]
			}
		},
		"TotalVisits": 317693541.4837979,
		"ReferralTraffic": 0.0037047,
		"TopPrompts": {
			"Status": 0,
			"ErrorMessage": null,
			"Prompts": [
				"What is the most popular search engine?",
				"How can I find information online?",
				"Where can I search for websites?"
			]
		}
	},
	"SnapshotDate": "2026-01-01T00:00:00+00:00",
	"timestamp": "2026-02-10T20:53:43.633Z"
}
```

## Understanding the Output

The actor returns a comprehensive JSON object with the following main sections:

### Basic Information
- `SiteName`: The domain name (e.g., "google.com")
- `Title`: Website title
- `Description`: Site description
- `Category`: Industry category classification
- `GlobalRank`: Overall global ranking (e.g., rank #1)

### Traffic & Engagement Metrics
```json
"Engagments": {
  "BounceRate": "0.28358483196353707",
  "PagePerVisit": "8.516282675924494",
  "Visits": "85756574615",
  "TimeOnSite": "610.4100441975721",
  "Month": "1",
  "Year": "2026"
}
```

- **BounceRate**: Percentage of visitors who leave after viewing only one page
- **PagePerVisit**: Average number of pages viewed per session
- **Visits**: Total monthly visits
- **TimeOnSite**: Average time spent on site (in seconds)

### Geographic Distribution
The `TopCountryShares` array shows the top 5 countries by traffic:

```json
{
  "country": "United States of America",
  "countryCode": "US",
  "Value": 0.24590223044328374,
  "valueinPercentage": "24.59"
}
```

### Traffic Sources
Shows where visitors come from:
- **Direct**: Visitors who type the URL directly
- **Search**: Traffic from search engines
- **Social**: Social media platforms
- **Referrals**: Other websites linking to this site
- **Mail**: Email links
- **Paid Referrals**: Paid advertising

### Top Keywords
Lists the most valuable search terms driving traffic:
```json
{
  "Name": "gmail",
  "EstimatedValue": 95585130,
  "Volume": 120497090,
  "Cpc": 1.74
}
```

- **Name**: The keyword/search term
- **EstimatedValue**: Estimated traffic value
- **Volume**: Monthly search volume
- **Cpc**: Cost per click in advertising

### AI Traffic Analytics
A unique feature showing traffic from AI chatbots:

```json
"AiTrafficDetails": {
  "Traffic": {
    "Split": [
      {"Name": "chatgpt.com", "Rank": 1},
      {"Name": "perplexity.ai", "Rank": 2},
      {"Name": "claude.ai", "Rank": 3}
    ]
  }
}
```

Tracks referral traffic from AI assistants, helping you understand how AI is driving visitors to websites.

### Monthly Visit Trends
Historical data showing traffic evolution:
```json
"EstimatedMonthlyVisits": [
  {
    "date": "2025-11-01",
    "visits": 82284033110,
    "percentageChange": null
  },
  {
    "date": "2025-12-01",
    "visits": 84172772881,
    "percentageChange": 2.3
  }
]
```

## Use Cases

### 1. **Competitor Research**
Analyze competing websites to understand:
- Their traffic volumes and trends
- Geographic markets they serve
- Top performing keywords
- Traffic source strategies (SEO vs. paid vs. social)

**Example**: A marketing agency analyzing a client's top 5 competitors to identify market opportunities.

### 2. **Market Research**
Research potential markets or industries:
- Identify top players in a category
- Understand market size and trends
- Analyze geographic distribution

**Example**: An e-commerce startup researching the online furniture market before launching.

### 3. **SEO Strategy**
Improve your search engine optimization:
- Discover high-value keywords competitors rank for
- Understand organic vs. paid traffic distribution
- Identify content opportunities

**Example**: An SEO specialist finding keyword gaps to target for a client website.

### 4. **Partnership Opportunities**
Identify potential partners or acquisition targets:
- Find websites in complementary niches
- Assess traffic quality and engagement
- Evaluate audience overlap

**Example**: A SaaS company looking for integration partners with similar user demographics.

### 5. **Due Diligence**
Verify claims during business transactions:
- Validate traffic numbers before acquiring a website
- Assess website value and monetization potential
- Verify growth claims with historical data

**Example**: An investor verifying traffic claims before purchasing a content website.

### 6. **Content Strategy**
Plan content based on search demand:
- Identify trending topics in your niche
- Understand what content drives traffic
- Discover engagement patterns

**Example**: A blogger planning an editorial calendar based on high-traffic topics.

### 7. **Media Buying & Advertising**
Make informed advertising decisions:
- Identify high-traffic sites for ad placement
- Understand audience demographics
- Evaluate ROI potential

**Example**: An ad network evaluating premium publisher opportunities.

### 8. **Performance Benchmarking**
Compare your website against industry standards:
- Track your ranking improvements
- Monitor engagement metrics vs. competitors
- Set realistic growth goals

**Example**: A startup tracking monthly progress against established competitors.

### 9. **AI Traffic Analysis**
Understand how AI is impacting web traffic:
- Track referrals from ChatGPT, Claude, Perplexity, etc.
- Monitor the growing importance of AI-driven discovery
- Optimize for AI chatbot visibility

**Example**: A content publisher analyzing how AI assistants are becoming a traffic source.

## Practical Examples

### Example 1: Analyzing a News Website
**Input**: `https://www.nytimes.com/`

**What You'll Learn**:
- Daily traffic volume and trends
- Geographic readership distribution
- Engagement metrics (how long people read)
- Top performing article topics
- Social media vs. direct traffic ratios

### Example 2: E-commerce Competitor Analysis
**Input**: `https://www.amazon.com/`

**What You'll Learn**:
- Market dominance and global reach
- Traffic sources (how they acquire customers)
- Seasonal trends in visits
- Geographic expansion strategy
- Keyword strategy for product categories

### Example 3: SaaS Tool Research
**Input**: `https://www.notion.so/`

**What You'll Learn**:
- User acquisition channels
- Geographic market penetration
- Organic search performance
- Competitor landscape
- Growth trajectory

## Best Practices

### 1. **Run Regular Comparisons**
- Track the same websites monthly to identify trends
- Create a dataset of competitors for ongoing analysis
- Monitor seasonal patterns

### 2. **Combine with Other Data Sources**
- Cross-reference with Google Analytics (for your own site)
- Use alongside keyword research tools
- Integrate with CRM data for complete picture

### 3. **Focus on Relevant Metrics**
- Don't get overwhelmed by all the data
- Choose 3-5 key metrics for your use case
- Track changes over time, not just absolute numbers

### 4. **Consider Data Limitations**
- Similarweb estimates may not be 100% accurate
- Smaller sites may have less reliable data
- Use as directional guidance, not absolute truth

### 5. **Respect Data Usage**
- Use data for research and analysis
- Don't violate terms of service
- Cite Similarweb when sharing insights publicly

## Data Export & Integration

### Exporting Data
The actor supports multiple export formats:
- **JSON**: Best for programmatic use and APIs
- **CSV**: Perfect for Excel and Google Sheets
- **Excel**: Ready-to-use spreadsheets
- **HTML**: Web-friendly format
- **RSS**: For feed readers

### API Integration
Access results programmatically using Apify's API:

```javascript
// Example: Fetching results via Apify API
const run = await client.actor('YOUR_ACTOR_ID').call({
  url: 'https://www.example.com/'
});

const dataset = await client.dataset(run.defaultDatasetId).listItems();
console.log(dataset.items);
```

### Scheduling Runs
Set up automatic weekly or monthly runs:
1. Go to actor settings
2. Click "Schedule"
3. Set frequency (daily, weekly, monthly)
4. Get automatic updated data without manual intervention

## Troubleshooting

### Common Issues

**Issue**: "URL query is required" error
- **Solution**: Make sure you've entered a URL in the input field

**Issue**: No data returned
- **Solution**: The website might be too small or new for Similarweb tracking. Try a larger, more established website.

**Issue**: Unexpected domain extracted
- **Solution**: The actor automatically extracts the root domain. If you want a subdomain analyzed, it will analyze the main domain instead.

**Issue**: Data seems outdated
- **Solution**: Similarweb data typically has a 1-2 month lag. Check the `SnapshotDate` field to see when data was collected.



## Pricing & Credits

This actor consumes Apify platform credits based on:
- Compute time (usually minimal - seconds per run)
- Data storage (if you save large amounts of results)

**Typical cost**: Very low - usually just a few cents per analysis or free on free tier.


## Changelog

### Version 1.0
- Initial release
- Domain extraction from URLs
- Comprehensive analytics retrieval
- AI traffic tracking
- Multiple export formats

---

## Quick Start Summary

1. **Enter a URL** → Any website you want to analyze
2. **Click Start** → Actor runs for a few seconds
3. **View Results** → Get comprehensive analytics data
4. **Export** → Download in your preferred format
5. **Take Action** → Use insights for strategy, research, or decisions

That's it! You now have professional-grade website analytics at your fingertips.


## Support


If you have any questions or encounter any issues, please consult the Apify documentation or reach out to us through one of the following channels:

* **Telegram**: [@pintoflow](https://t.me/pintoflow)
* **Email**: [pintoflowpt@gmail.com](mailto:pintoflowpt@gmail.com)
* **Apify Platform**: You can also contact us directly through this platform.

---

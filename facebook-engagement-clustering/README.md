# Customer Engagement Clustering — Facebook Marketplace Data

Applied K-Means clustering to segment Facebook posts from Thai retail sellers based on user engagement patterns.

## Dataset
~7,000 Facebook posts with engagement metrics: reactions, comments, shares, and reaction-type breakdowns (likes, loves, wows, hahas, sads, angrys), across four post types — photo, video, status, and link.

## Approach
- Cleaned and explored the dataset, examining the distribution of post types
- Selected relevant engagement features for clustering
- Used the elbow method to determine the optimal number of clusters
- Applied K-Means clustering to group posts by engagement pattern
- Analyzed how engagement (reactions, comments, shares) varied across clusters and post types

## Key Findings
- Photo and video posts made up the large majority of content (photo: ~4,300, video: ~2,300)
- Distinct engagement clusters emerged, separating high-engagement viral-style posts from typical low-engagement posts
- Reaction counts showed strong internal correlation with likes, while comments and shares behaved more independently across clusters

## Tools
Python, Pandas, Scikit-learn, Matplotlib

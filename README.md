# URL Feature Extraction Project

This project aims to extract various features from URLs using machine learning techniques to identify potential phishing attempts. The project involves several steps:

### Data Loading and Preparation

- Loads phishing and legitimate URLs from CSV files
- Combines the datasets into a single DataFrame
- Converts the combined data to JSON format for easier manipulation

### Feature Extraction

The project extracts several features from each URL:

1. Basic Features:
   - Domain extraction
   - IP address detection
   - Length of the URL
   - Depth of the URL path
   - Presence of redirection symbols
   - Protocol (HTTP/HTTPS)
   - URL shortening detection
   - Presence of prefix/suffix in domain

2. DNS and WHOIS Information:
   - DNS records
   - Whois record details
   - Age of the domain
   - End period of the domain

3. HTML-based Features:
   - IFrame redirection
   - Status bar customization
   - Disabling right-click functionality
   - Website forwarding

### Implementation Details

- Uses Dask for parallel processing of large datasets
- Utilizes Python libraries such as pandas, json, urllib, socket, and whois
- Implements regular expressions for pattern matching in HTML content

### Usage

To run the project:

1. Install required dependencies:

2. Execute the notebook to generate the extracted features

### Output

The project generates a JSON file containing the original URLs along with their extracted features. This output can be further analyzed using machine learning algorithms to classify URLs as phishing or legitimate.

### Future Improvements

- Implement more advanced feature extraction techniques
- Integrate with machine learning models for classification
- Add visualization components for better insights
- Optimize performance for larger datasets

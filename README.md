Product Card Enhancements

Changes Implemented:

Secondary Hover Images by Variant:
Implemented a hover effect that shows an alternate image for the selected variant on product cards. Uses a naming convention on the product media alt text (e.g., Classic T shirt - Green - Side view) to map secondary images to color variants.


Data & Fallback Logic:

Data Source: Alt text of product media, following the pattern Product Name - Color - View.

Mapping to Variants: The system extracts the variant color from the selected option and matches it to an image whose alt text contains that color.

Fallback:

If no secondary image is found for the variant, the hover defaults to the main product image.

Variant selection always updates both the displayed image and product link URL.

Notes:

No additional metafields were added; the solution relies entirely on alt text conventions.

All updates are scoped to the product card component (product-card.js)

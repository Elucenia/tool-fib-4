<!-- ELUCENIA technical documentation · fib-4 · hi · no clinical/professional/rights approval -->

# FIB-4 (लिवर फाइब्रोसिस)

[शर्तें, स्रोत और अनुमतियाँ](https://elucenia.org/hi/tools/fib-4)

## उपयोग कैसे करें

पोर्टल पर उपकरण का उपयोग करें या स्थानीय HTTP सर्वर के माध्यम से index.html खोलें। भाषा चुनें, फ़ील्ड भरें और गणना करें।

## इनपुट और इकाइयाँ

### आयु

`idade`

वर्ष · सीमा: 18–100

### AST

`ast`

U/L · सीमा: 1–5000

### ALT

`alt`

U/L · सीमा: 1–5000

### प्लेटलेट्स

`plq`

× 10³/mm³ · सीमा: 5–1500

### संदर्भ

`etio`

- `masld` — स्टीएटोसिस (MASLD/NAFLD)
- `viral` — हेपेटाइटिस C या HIV/HCV

## विधि का संस्करण

FIB-4/Sterling 2006; HCV/HIV सीमाएँ 1.45/3.25 बनाम MASLD 1.3/2.67 और ≥65 वर्ष 2.0

## दस्तावेज़ित सूत्र

FIB-4 = (आयु × AST) ÷ (प्लेटलेट्स \[10⁹/L\] × √ALT)।

MASLD: \< 1.30 उन्नत फ़ाइब्रोसिस को नकारता है (65 वर्ष से \< 2.0); \> 2.67 उन्नत फ़ाइब्रोसिस सुझाता है। हेपेटाइटिस C/HIV: \< 1.45 और \> 3.25।

## सीमाएँ और जनसमूह

Sterling 2006 FIB-4 का विकास HIV/HCV सह-संक्रमित रोगियों में हुआ था; \<1.45 और \>3.25 कटऑफ को Ishak 4–6 फाइब्रोसिस के विरुद्ध परखा गया। सूत्र आयु वर्ष में, AST और ALT U/L में तथा प्लेटलेट्स 10^9/L में उपयोग करता है। ये कटऑफ और मूल आबादी MASLD मानदंड या आयु-संशोधनों के साथ स्वचालित रूप से परस्पर बदलने योग्य नहीं हैं; उन संस्करणों के अपने स्रोत आवश्यक हैं।

## संदर्भ

- [Sterling RK et al. Development of a simple noninvasive index to predict significant fibrosis in patients with HIV/HCV coinfection. Hepatology, 2006.](https://doi.org/10.1002/hep.21178)

- [Shah AG et al. Comparison of noninvasive markers of fibrosis in patients with nonalcoholic fatty liver disease. Clin Gastroenterol Hepatol, 2009.](https://doi.org/10.1016/j.cgh.2009.05.033)

- [McPherson S et al. Age as a confounding factor for the accurate non-invasive diagnosis of advanced NAFLD fibrosis. Am J Gastroenterol, 2017.](https://doi.org/10.1038/ajg.2016.453)

- [Rinella ME et al. AASLD Practice Guidance on the clinical assessment and management of nonalcoholic fatty liver disease. Hepatology, 2023.](https://doi.org/10.1097/HEP.0000000000000323)

## तकनीकी परीक्षण दोहराएँ

दर्ज कृत्रिम मामलों को दोहराने के लिए इस रिपॉज़िटरी की मूल निर्देशिका में node test.cjs चलाएँ। मूल इनपुट, अपेक्षित परिणाम और सहनशीलता सीमाएँ सुरक्षित रखी गई हैं। तकनीकी परीक्षण नैदानिक सत्यापन नहीं हैं।

```sh
node test.cjs
```

tool.json में स्रोत, संस्करण और समीक्षा का दायरा दिया गया है। examples.json में कृत्रिम इनपुट और अपेक्षित परिणाम सुरक्षित हैं; results.json में प्राप्त परिणाम दर्ज हैं।

[रिकॉर्ड और संदर्भ](../tool.json) · [JavaScript कोड](../calculator.js) · [संदर्भ मामले](../examples.json) · [results.json](../results.json)

## समीक्षा और उपयोग की शर्तें

स्वतंत्र नैदानिक समीक्षा नहीं की गई है।

यह इंटरफ़ेस लेखकों द्वारा किया गया अनुवाद है, कोई आधिकारिक या प्रमाणित संस्करण नहीं। स्वतंत्र नैदानिक समीक्षा, पेशेवर भाषाई समीक्षा और उपकरणों के अधिकारों की अनुमति की प्रक्रिया पूरी नहीं हुई है।

सूत्र या वर्गीकरण का परिणाम। व्याख्या, कार्यवाही और उपयुक्तता पेशेवर मूल्यांकन और चुने गए स्रोत पर निर्भर है।

## लाइसेंस और श्रेय

Apache-2.0 केवल ELUCENIA के कोड पर लागू होता है। उपकरणों, प्रकाशनों, अनुवादों और डेटा के अधिकार उनके संबंधित अधिकारधारकों के पास रहते हैं। LICENSE और NOTICE सुरक्षित रखें।

ELUCENIA · Felipe Guedes · Copyright © 2026

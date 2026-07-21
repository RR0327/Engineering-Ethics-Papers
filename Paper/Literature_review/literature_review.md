# LITERATURE REVIEW

The study of user data collection, deceptive user interface (UI) design, and informed consent encompasses software engineering, human-computer interaction (HCI), behavioral economics, and data privacy law. This review synthesizes empirical findings, taxonomies, and technical analyses from key research literature to contextualize how modern web and mobile applications manipulate choice architecture and extract user telemetry.

### A. Taxonomies and Large-Scale Empirical Detection of Dark Patterns

* **Taxonomic Frameworks:** Nie et al. proposed the Dark Pattern Analysis Framework (DPAF). Through a systematic literature review, they developed a taxonomy containing 64 dark-pattern types across 6 categories and 31 subcategories. Their evaluation showed that five existing detection tools could identify only 32 of the 64 types, resulting in 50% coverage. Existing benchmark datasets similarly covered only 32 types, limiting the effectiveness of automated classification systems [[8]](#reference-8).

* **Web-Scale Measurement:** Mathur et al. crawled approximately 53,000 product pages across 11,000 shopping websites using OpenWPM and text-clustering techniques. They identified 1,818 dark-pattern instances across 11.1% of the sampled websites and found that more popular websites were more likely to contain such designs. The study also identified 22 third-party organisations supplying ready-made dark-pattern services to online retailers [[2]](#reference-2).

### B. Compliance, Consent Architecture, and Telemetry Leakage

* **Web-Based Consent Management Platforms:** Nouwens et al. examined 680 implementations of the five most widely used consent-management platforms across popular UK websites. Only 11.7% met the authors’ three minimum requirements: explicit consent, equal effort for acceptance and rejection, and no optional pre-ticked boxes. Their controlled experiment with 40 participants showed that removing the “Reject All” option from the first interface layer increased consent by 22–23 percentage points [[1]](#reference-1).

* **News Media Cookie-Consent Interfaces:** Soe et al. manually examined 300 cookie-consent notices from Scandinavian and English-language news outlets. They found dark patterns in 297 notices, with obstruction and interface interference being the dominant categories. Only 15 websites provided a direct one-click rejection option, while all provided one-click acceptance. Half of the websites required 10–12 clicks to reject all cookies. The authors also identified eight consent-specific patterns, including choice cascades, widget inequality, and unlabeled sliders [[5]](#reference-5).

* **Mobile Ecosystem Telemetry and Consent:** Koch et al. analysed 3,006 Android and 1,773 iOS applications. Only 22.3% displayed any privacy-consent dialogue, while only 11.9% offered users an actionable choice. Among the detected dialogues, 98.4% on Android and 99.5% on iOS violated at least one of the authors’ design requirements for valid and non-coercive consent. The authors clarified that these design violations do not automatically establish GDPR violations. Their traffic analysis also found that 94.2% of observed network requests occurred before any interaction with the consent dialogue [[3]](#reference-3).

### C. Permission Rationales and Front-End Choice Architecture

* **Permission-Rationale Impact:** Elbitar et al. analysed approximately 770,000 URLs and identified around 3,674 unique rationale texts and 749 rationale-interface designs across approximately 85,000 webpages. Overlays presented before or alongside browser prompts were associated with a 41% increase in permission-grant rates, while full-screen rationales were associated with a 33% increase [[4]](#reference-4).

* **Framing and User Sentiment:** Elbitar et al. found that positive and neutral rationale messages increased permission-grant rates by 18% and 8%, respectively. In contrast, consequence-based messages emphasising what users might lose were associated with a 20% reduction in grant rates and a 12% increase in dismissals. Dialog and text rationales were also associated with increased user annoyance in some contexts [[4]](#reference-4).

### D. Information Asymmetry and Human Psychological Vulnerability

* **Information Asymmetry and Policy Comprehension:** Bashir et al. conducted a knowledge survey with 455 participants and an opinion and online-behaviour survey with 756 participants. They found that 44% did not know that free websites could profit by selling user information directly to marketing companies, while 25% failed to answer a basic question about the fundamental nature of cloud computing. Furthermore, 81% reported submitting information online even though they wished they had not been required to do so, indicating limited voluntariness in online consent [[6]](#reference-6).

* **User Perception and the Limits of Awareness:** Bongard-Blanchy et al. surveyed 406 users and found that 59% correctly identified at least five dark patterns across nine manipulative interfaces. General awareness did not significantly predict resistance to manipulation, although stronger dark-pattern recognition was associated with a lower reported likelihood of influence. The findings suggest that awareness alone is insufficient to protect users from manipulative interface designs [[7]](#reference-7).

### E. Ethical Frameworks and Engineering Dilemmas

* **Design Dilemmas:** Simon et al. identified three major ethical dilemmas: whether manipulation can be justified when intended to produce beneficial outcomes, how designers should balance individual welfare against societal welfare, and how excessive transparency or choice can create information overload rather than meaningful autonomy [[9]](#reference-9).

* **Rational-Choice Principles:** Simon et al. argued that both nudging and manipulative design often treat users as irrational actors whose cognitive biases should either be corrected or exploited. They proposed interface-design principles that treat users as rational decision-makers and support deliberate, autonomous choices through approaches such as boosting and value-sensitive design [[9]](#reference-9). Equal visual and interaction treatment of acceptance and rejection options is more directly supported by Nouwens et al. [[1]](#reference-1) and Soe et al. [[5]](#reference-5).

# REFERENCES

<a id="reference-1"></a>
**[1]** M. Nouwens, I. Liccardi, M. Veale, D. Karger, and L. Kagal, “Dark Patterns Post-GDPR: Scraping Consent Interface Designs and Demonstrating their Influence,” in *Proceedings of the 2020 CHI Conference on Human Factors in Computing Systems (CHI ’20)*, 2020.

<a id="reference-2"></a>
**[2]** A. Mathur, G. Acar, M. J. Friedman, E. Lucherini, J. Mayer, M. Chetty, and A. Narayanan, “Dark Patterns at Scale: Findings from a Crawl of 11K Shopping Websites,” *Proceedings of the ACM on Human-Computer Interaction*, vol. 3, no. CSCW, Art. no. 81, 2019.

<a id="reference-3"></a>
**[3]** S. Koch, B. Altpeter, and M. Johns, “The OK Is Not Enough: A Large-Scale Study of Consent Dialogs in Smartphone Applications,” in *Proceedings of the 32nd USENIX Security Symposium*, 2023.

<a id="reference-4"></a>
**[4]** Y. Elbitar, S. Khodayari, M. Harbach, G. De Stefano, B. C. Engedy, G. Pellegrino, and S. Bugiel, “Permission Rationales in the Web Ecosystem: An Exploration of Rationale Text and Design Patterns,” in *Proceedings of the 2025 CHI Conference on Human Factors in Computing Systems (CHI ’25)*, 2025.

<a id="reference-5"></a>
**[5]** T. H. Soe, O. E. Nordberg, F. Guribye, and M. Slavkovik, “Circumvention by Design—Dark Patterns in Cookie Consents for Online News Outlets,” arXiv:2006.13985, 2020.

<a id="reference-6"></a>
**[6]** M. Bashir, C. Hayes, A. D. Lambert, and J. P. Kesan, “Online Privacy and Informed Consent: The Dilemma of Information Asymmetry,” in *Proceedings of the Association for Information Science and Technology Annual Meeting (ASIS&T)*, 2015.

<a id="reference-7"></a>
**[7]** K. Bongard-Blanchy, A. Rossi, S. Rivas, S. Doublet, V. Koenig, and G. Lenzini, “‘I am Definitely Manipulated, Even When I am Aware of it. It’s Ridiculous!’—Dark Patterns from the End-User Perspective,” in *Proceedings of the 2021 ACM Designing Interactive Systems Conference (DIS ’21)*, 2021.

<a id="reference-8"></a>
**[8]** L. Nie, Y. Zhao, C. Li, X. Luo, and Y. Liu, “Shadows in the Interface: A Comprehensive Study on Dark Patterns,” *Proceedings of the ACM on Software Engineering*, vol. 1, no. FSE, Art. no. 10, 2024.

<a id="reference-9"></a>
**[9]** M.-S. Simon, H. Schraffenberger, and R. Gellert, “Influencing User Decisions: Dilemmas in Designing Online Interfaces,” in *Adjunct Proceedings of the 2024 Nordic Conference on Human-Computer Interaction (NordiCHI Adjunct ’24)*, 2024.

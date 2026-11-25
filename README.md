# From Keywords to Context

**A conceptual research paper arguing that domain-specific retrieval-augmented generation (RAG) is the next step for enterprise knowledge management, and that whether it works depends more on people than on the technology.**

*Knowledge Management & Business Intelligence (ISM 6255) · Seattle Pacific University · June 2026*

---

## The question

Organizations hold huge amounts of knowledge, and people still can't find the right piece when they need it. For decades the retrieval layer of knowledge repositories has been keyword search, and keyword search is well documented to miss a lot.

So I asked: can domain-specific RAG, built on a curated, authoritative corpus instead of the open internet, fix the retrieval problem knowledge management (KM) has been stuck on for decades? And what does it still leave unsolved?

## Approach

This is a conceptual paper. There's no dataset or code here. I brought three bodies of work together:

- **Classical KM theory:** Nonaka's SECI model, Davenport & Prusak, Alavi & Leidner, and Dalkir's KM cycle
- **The case against keyword retrieval:** Blair & Maron (1985), Blair (2002), and Corral, LaBrie & St. Louis (2005)
- **Recent peer-reviewed RAG evidence,** mostly from biomedicine: Lewis et al. (2020), Gao et al. (2023), the Ke et al. (2025) meta-analysis, Amugongo et al. (2024), and Kumar et al.'s (2026) review of enterprise RAG

I mapped RAG onto KM theory, then tested the argument against the organizational research on subcultures (Ravishankar et al., 2011) and human values (Tams et al., 2020).

## Key points

> Domain-specific RAG is a credible next evolution of enterprise KM infrastructure. RAG handles the technical side well; the human side is still up to us.

- **RAG fits KM theory.** The vector database holds externalized explicit knowledge (the Combination step in SECI). The retriever acts like a librarian who gets what you mean. The LLM turns what it finds into one answer you can act on (Internalization).
- **It swaps recall for recognition.** Keyword search makes you guess the exact words a document uses. RAG lets you describe your problem in plain language and recognize the answer. It's the same insight behind Corral et al.'s 2005 visual keyword hierarchies, taken one step further.
- **The corpus is the big design decision.** Grounding answers in vetted sources is what cuts hallucination. Across 20 biomedical studies, Ke et al. (2025) found an overall odds ratio of 1.35 in favor of RAG. A controlled corpus also lets you enforce document-level permissions at retrieval.
- **It targets three old KM problems:** retrieval failure, hallucination, and knowledge walking out the door when experts leave.
- **The tech is the easy part.** The same system can succeed in one team and fail in another (Ravishankar et al., 2011), and people's values predict how much they use and contribute to a knowledge repository (Tams et al., 2020). Organizations that treat RAG as a knowledge governance project, not a tech project, are the ones likely to succeed.

## What it doesn't solve

- Tacit knowledge stays out of reach. RAG can spread what's written down, but it can't replace apprenticeship.
- A RAG system is only as good as its corpus, and corpus quality decays without upkeep.
- Peer-reviewed evidence from real enterprise deployments is still thin next to academic prototypes (Kumar et al., 2026).

## Where I'd take it next

Field studies of enterprise RAG rollouts; whether semantic retrieval eases or worsens subculture resistance; hybrid vector + knowledge-graph retrieval in a KM setting; and applying the Tams et al. values framework to RAG adoption.

## Read it

📄 **[Full paper (PDF)](paper/From-Keywords-to-Context_Kinoti_2026.pdf)** · 21 pages, APA. Appendix A lists the generative AI prompts I used while researching and writing it.

## Repo layout

```
rag-knowledge-management-paper/
├── README.md
└── paper/
    └── From-Keywords-to-Context_Kinoti_2026.pdf
```

---

*Brenda Kinoti · MS Data Analytics & Business, Seattle Pacific University · [Portfolio](https://brendakinoti-datascientist.netlify.app)*

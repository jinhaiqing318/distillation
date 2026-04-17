---
name: gepengfei-stock-judge
description: "analyze a stock using a distilled gepengfei-style framework derived from his article corpus. use when the user uploads stock information, company notes, research snippets, announcements, or a self-written stock memo and wants a sharp gepengfei-style analysis, a direct judgment on whether the stock can be bought now, watched, or avoided, and a clear separation between long-term logic and short-term theme logic in a-shares."
---

# gepengfei stock judge

## Overview
Read the user's stock materials, reconstruct the strongest investable logic, then judge the stock in a voice and reasoning style close to 葛鹏飞. Favor a sharp, direct conclusion over vague balance. Distinguish clearly between “能不能买” and “是不是中长线”.

## Workflow

### 1. Normalize the input
Treat any uploaded stock material as raw clues, not truth. Extract only what matters for a buy decision:
- company identity and ticker
- business and revenue drivers
- industry trend and timing
- orders, customers, products, capacity, mergers, policy links, or catalysts
- valuation, if provided
- market sentiment and recent price behavior, if provided

If the user provides too little information, still give a provisional judgment based on what is present. Say what is missing instead of pretending certainty.

### 2. Classify the stock before judging it
Force the stock into one primary bucket first:
- growth stock
- cycle / macro-sensitive stock
- policy / state-owned / resource stock
- merger or restructuring story
- pure theme / sentiment trade
- mature value stock with weak growth

This step is mandatory. Many bad judgments come from using the wrong framework on the wrong stock.

### 3. Apply the gepengfei lens
Use the following rules aggressively.

#### A. Logic beats stories
Prefer causal chains, industrial facts, and incentives over slogans. If the thesis depends mainly on phrases like “the next xx”, “big imagination”, “national support”, or “everyone knows this will explode”, treat that as weak evidence.

#### B. Separate 中长线 from 题材
A stock is not a 中长线 candidate just because the chart is strong or the policy tone is warm. Ask:
- does it have real growth space?
- is it standing near an industry expansion point?
- does the company have a durable position, not just a market nickname?
- if sentiment cools, does the core thesis still stand?

If the answer is weak, label it as 题材 or trading opportunity, not 中长线.

#### C. Growth matters more than “big and stable” in equity investing
Repeatedly ask whether the company can become materially larger. In this framework, capital markets exist mainly to fund future growth. If a company is large, mature, policy-protected, but structurally low-growth, do not pretend it is a compelling long-term equity story.

#### D. Hot sectors and hot leaders are dangerous
Be skeptical of the hottest stock in the hottest track, especially when the crowd extrapolates far into the future. If expectations are already too full, say so directly.

#### E. Avoid weak-quality equity stories
Mark down or reject stocks with one or more of these traits:
- dependence on whispered “inside information”
- overreliance on one major customer
- fashionable or exaggerated branding with weak substance
- unfocused diversification
- old industry, weak growth, yet expensive valuation
- thesis relies mainly on policy support without strong economics

#### F. Qualitative insight can matter more than spreadsheets
Do not hide behind ratios when the key question is industrial positioning, credibility, order quality, management incentives, or whether the company sits at the front edge of an expansion wave. But do not use this as an excuse for fantasy. Qualitative judgment must still point to a concrete mechanism.

#### G. In a-shares, structure and timing matter
For A-shares, always discuss whether the opportunity is driven by:
- industry boom
- liquidity / sentiment
- policy wind
- anti-involution / supply reform / macro rotation
- merger and restructuring expectation

Do not talk about the stock as if it trades in a vacuum.

#### H. Position sizing is part of the answer
If the logic is only medium-strength, do not give a full-throated “buy”. Use three levels:
- can buy now
- can watch / wait for better price or evidence
- should not buy now

Optionally add a light position view such as “only suitable for small position tracking” or “not suitable for heavy仓”.

### 4. Write in the target style
Write with these stylistic traits:
- direct judgment first, nuance second
- rhetorical questions are welcome when exposing weak logic
- short, punchy paragraphs
- willing to say “this is only a theme” or “this is not a long-term line”
- use plain language, not sell-side jargon stacking
- occasional sharpness or irony is acceptable, but do not become vulgar
- sound like a person making a real market call, not a neutral memo

Do not fabricate private facts, management conversations, or insider information. If the user did not provide evidence, say it is unknown.

## Output format
Use exactly this structure unless the user asks for another format.

### 1. 论证风格分析
Write 4 to 8 short paragraphs in a 葛鹏飞-style voice. The section should:
- identify the stock type
- expose the strongest logic
- attack the weakest logic
- separate industry truth from market emotion
- say whether it is 中长线 or merely a 题材 / 波段机会

### 2. 能不能买
End with one explicit line chosen from the following:
- 结论：可以买，但只适合……
- 结论：可以观察，暂时不急着买。
- 结论：不能买，至少现在不能。

Then add 2 to 4 bullets:
- why
- what would change the conclusion
- biggest risk
- if relevant, whether the judgment is about 中长线 or only交易

## Default evaluation checklist
Silently check these items before concluding:
1. what kind of stock is this?
2. what exactly is the growth engine?
3. where is the company in the industry chain?
4. does it have order, product, customer, or capacity evidence?
5. is the market already pricing the story too fully?
6. is this a long-term equity thesis or only a theme?
7. what is the biggest disconfirming fact?

## Boundary rules
- Never present certainty when the input is thin.
- Never recommend leverage, all-in behavior, or reckless concentration.
- If the user only uploads noisy sentiment material with little company information, say the evidence is insufficient.
- If the material supports both a trading thesis and a long-term thesis, separate them explicitly.
- If the stock is mainly policy-propped, state that policy can create行情 but not necessarily durable equity value.

## Resources
Use these bundled references when needed:
- `references/gepengfei-framework.md` for the distilled investment lens
- `references/output-template.md` for the standard answer pattern

---
layout: "page"
title: Example API Response
nav_order: 5
parent: Making a Call to the Receptiviti API

---

# Example API Response

```
{
  "db_id": null,
  "content_handle": "string",
  "content_source": 0,
  "content_date": "2020-01-05T00:00:00",
  "content_tags": [
    "string"
  ],
  "user_id": 185,
  "user": {
    "name": "your name",
    "email": "name@address.com",
    "first_name": "your",
    "last_name": "name",
    "company_name": "company_name",
    "job_title": null,
    "has_twitter_api_access": false,
    "is_on_trial": false,
    "status": "active",
    "rate_limit": "150000000/month"
  },
  "language": "english",
  "organa_scores": {},
  "word_count": 308,
  "receptiviti_scores": {
    "percentiles": {
      "openness": 60.35874031001012,
      "conscientiousness": 47.63460475709875,
      "extraversion": 68.61794649270975,
      "agreeableness": 23.770726094706376,
      "neuroticism": 38.26375176692578,
      "artistic": 70.74024541968724,
      "adventurous": 70.72719108084947,
      "intellectual": 65.31664106266301,
      "liberal": 45.957687012634096,
      "imaginative": 39.57805467483369,
      "emotionally_aware": 46.30843865524487,
      "sociable": 45.112194922805394,
      "friendly": 83.02507507551876,
      "assertive": 17.364791154191956,
      "active": 80.06300986133593,
      "energetic": 66.77543339169682,
      "cheerful": 54.67424200232799,
      "self_assured": 77.96717129846508,
      "disciplined": 67.13124382113041,
      "ambitious": 36.78308996025509,
      "dutiful": 29.99389100240535,
      "cautious": 31.288680832320235,
      "organized": 62.66400494525187,
      "generous": 23.24624850071529,
      "trusting": 84.41802904003006,
      "cooperative": 53.149400064511816,
      "empathetic": 11.481695213584484,
      "genuine": 36.955079584878355,
      "humble": 40.320633971838404,
      "impulsive": 56.89544953967971,
      "stressed": 29.20378120375311,
      "anxious": 27.786171293008113,
      "aggressive": 81.33069167632283,
      "melancholy": 31.828787894900586,
      "self_conscious": 25.06640787742607,
      "thinking_style": 3.8032533389566767,
      "power_driven": 67.63499187332971,
      "independent": 9.880557192423902,
      "cold": 90.55574033810831,
      "insecure": 29.32309941503369,
      "adjustment": 1,
      "happiness": 22.018651756520708,
      "persuasive": 67.98006007519217,
      "social_skills": 83.18347675664145,
      "type_a": 34.46151622954636,
      "depression": 43.8910030132187,
      "workhorse": 1.4133527919919986,
      "family_oriented": 11.309620894425493,
      "reward_bias": 60.95456730769231,
      "friend_focus": 30.301344646823317,
      "body_focus": 67.34647608497133,
      "health_oriented": 25.687734709530453,
      "sexual_focus": 38.59850307933812,
      "food_focus": 36.90316610452883,
      "leisure_oriented": 37.23078470899094,
      "money_oriented": 58.45563972756394,
      "religion_oriented": 99,
      "work_oriented": 47.03203172773348,
      "netspeak_focus": 23.812132689852675
    },
    "raw_scores": {
      "openness": 1.1381982786635403,
      "conscientiousness": 0.4331444349331217,
      "extraversion": 1.151019173645724,
      "agreeableness": -5.799592314432606,
      "neuroticism": 0.8613844854703785,
      "artistic": 3.5573806948833036,
      "adventurous": 2.492331694615021,
      "intellectual": 9.930704352917726,
      "liberal": 0.036949369178082225,
      "imaginative": -1.182944827904076,
      "emotionally_aware": 1.3713064471476208,
      "sociable": 2.872627241081873,
      "friendly": 4.24403300418768,
      "assertive": 0.5079245123264008,
      "active": -0.24593132029061893,
      "energetic": 1.7109593148501365,
      "cheerful": 1.3435768691848762,
      "self_assured": 2.8579344256071906,
      "disciplined": 2.577478860991675,
      "ambitious": 3.143995396183884,
      "dutiful": -3.349628602220175,
      "cautious": 0.9145783802816903,
      "organized": 0.6064343807040871,
      "generous": -3.5398819963543335,
      "trusting": 1.9215385210592864,
      "cooperative": 4.100687975963773,
      "empathetic": -2.9132711056667957,
      "genuine": -1.5526738294215534,
      "humble": -1.5675117360686865,
      "impulsive": 2.5128879079775173,
      "stressed": 3.367196595294918,
      "anxious": 1.0321819763436495,
      "aggressive": 6.026203943840621,
      "melancholy": -0.7087007028936146,
      "self_conscious": 0.6788997680043013,
      "thinking_style": -3.5245195222986343,
      "power_driven": 6.21943481254863,
      "independent": -7.34765098358293,
      "cold": 1.0354217482786114,
      "insecure": -0.13944606287367417,
      "adjustment": -7.1034745652133955,
      "happiness": 3.6889774875835117,
      "persuasive": -0.04440506424393842,
      "social_skills": 2.5031353972708006,
      "type_a": 6.975379446492398,
      "depression": 0.6557945613384311,
      "workhorse": -7.372384855283657,
      "family_oriented": 1.3799609741742578,
      "reward_bias": 1.6233766,
      "friend_focus": 0,
      "body_focus": 0.32467532,
      "health_oriented": 0,
      "sexual_focus": 0,
      "food_focus": 0,
      "leisure_oriented": 0.32467532,
      "money_oriented": 0.64935065,
      "religion_oriented": 0.9740259500000001,
      "work_oriented": 0.9740259500000001,
      "netspeak_focus": 0
    },
    "warnings": {
      "artistic": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "adventurous": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "intellectual": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "liberal": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "imaginative": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "emotionally_aware": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "sociable": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "friendly": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "assertive": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "active": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "energetic": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "cheerful": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "self_assured": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "disciplined": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "ambitious": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "dutiful": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "cautious": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "organized": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "generous": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "trusting": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "cooperative": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "empathetic": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "genuine": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "humble": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "impulsive": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "stressed": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "anxious": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "aggressive": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "melancholy": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ],
      "self_conscious": [
        "Insufficient word count. Requires a minimum of 500 words for accurate results."
      ]
    }
  },
  "liwc_scores": {
    "wc": 308,
    "analytic": 15.448536,
    "clout": 56.453506,
    "authentic": 54.98235,
    "tone": 83.48441,
    "wps": 11,
    "sixLtr": 0.14935064,
    "dic": 0.9253247,
    "categories": {
      "function": 0.6136364,
      "pronoun": 0.16558442,
      "ppron": 0.064935066,
      "i": 0.025974026,
      "we": 0,
      "you": 0.016233766,
      "shehe": 0,
      "they": 0.022727273,
      "ipron": 0.10064935,
      "article": 0.051948052,
      "prep": 0.10714286,
      "auxverb": 0.15584415,
      "adverb": 0.097402595,
      "conj": 0.055194806,
      "negate": 0.032467533,
      "verb": 0.23051947,
      "adj": 0.035714287,
      "compare": 0.016233766,
      "interrog": 0.022727273,
      "number": 0.016233766,
      "quant": 0.025974026,
      "affect": 0.045454547,
      "posemo": 0.038961038,
      "negemo": 0.0064935065,
      "anx": 0,
      "anger": 0.0032467532,
      "sad": 0,
      "social": 0.097402595,
      "family": 0,
      "friend": 0,
      "female": 0.0032467532,
      "male": 0,
      "cogproc": 0.17207792,
      "insight": 0.025974026,
      "cause": 0.042207792,
      "discrep": 0.012987013,
      "tentat": 0.038961038,
      "certain": 0.032467533,
      "differ": 0.038961038,
      "percept": 0.025974026,
      "see": 0.0064935065,
      "hear": 0.012987013,
      "feel": 0.0064935065,
      "bio": 0.0032467532,
      "body": 0.0032467532,
      "health": 0,
      "sexual": 0,
      "ingest": 0,
      "drives": 0.06818182,
      "affiliation": 0.0032467532,
      "achieve": 0.0064935065,
      "power": 0.045454547,
      "reward": 0.016233766,
      "risk": 0,
      "focuspast": 0.051948052,
      "focuspresent": 0.14935064,
      "focusfuture": 0.012987013,
      "relativ": 0.1396104,
      "motion": 0.029220778,
      "space": 0.07467532,
      "time": 0.048701297,
      "work": 0.0097402595,
      "leisure": 0.0032467532,
      "home": 0,
      "money": 0.0064935065,
      "relig": 0.0097402595,
      "death": 0,
      "informal": 0.016233766,
      "swear": 0,
      "netspeak": 0,
      "assent": 0.0032467532,
      "nonflu": 0.012987013,
      "filler": 0,
      "AllPunc": 0.2564935,
      "Period": 0.09415584,
      "Comma": 0.071428575,
      "Colon": 0,
      "SemiC": 0,
      "QMark": 0,
      "Exclam": 0,
      "Dash": 0.0032467532,
      "Quote": 0.045454547,
      "Apostro": 0.038961038,
      "Parenth": 0,
      "OtherP": 0.0032467532
    }
  },
  "personality_snapshot": [
    {
      "summary": "Poorly-adjusted",
      "description": "May exhibit questionable judgement, and their opinions may not be particularly grounded in facts and reality."
    },
    {
      "summary": "Nonchalant",
      "description": "May procrastinate or wait until deadlines approach before getting started. Seldom puts in extra time to complete projects."
    },
    {
      "summary": "Emotional thinking style",
      "description": "Tends to think in the here-and-now and bases decisions almost entirely on their feelings and intuition. Makes decisions quickly and may be resistant to changing their opinion."
    }
  ],
  "communication_recommendation": "Get to know them before getting to the point. Influence them by appealing to their emotions. Don't waste their time with small-talk. Be prepared to give advice and share your opinion.",
  "emotional_analysis": {
    "emotional_tone": {
      "score": 83.48441,
      "rating": "Positive"
    },
    "facets": {
      "sad": 0,
      "anger": 49.99999923,
      "fear": 0
    }
  },
  "_links": {}
}
```

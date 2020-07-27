---
title: 交易类型 # 课程标题
challengeType: 0               # 课程类型，默认为0：理论， 1： 实验
order: 1                       # 序号，以此为当前单元的课程排序
time:  5个小时                  # 学习时长
videoUrl: ''                   # 视频链接地址
prjectUrl: 'https://github.com/' # 源码地址
localeTitle: DDN交易类型       # 本地化标题
toc: menu
---

# 交易类型

交易类型是标明链上交易方式的标识符，由0~100数字表示，不能重复。DDN 区块链目前支持多种交易类型，列表如下：

```js
  // base 0-19
  TRANSFER: 0, // TRANSFER .TRANSFER
  SIGNATURE: 1, // SETUP SECOND_PASSWORD
  DELEGATE: 2, // DELEGATE
  VOTE: 3, // VOTE FOR DELEGATE
  MULTISIGNATURE: 4, // MULTISIGNATURE note: .MULTI -> .MULTISIGNATURE
  DAPP: 5, // DAPP REGISTER
  DAPP_IN: 6, // DAPP DEPOSIT
  DAPP_OUT: 7, // DAPP WITHDRAW

  MULTITRANSFER: 8, 
  USERINFO: 9,

  // Evidence: 20-39,
  EVIDENCE: 20,

  // DAO 40-59
  DAO_ORG: 40,
  DAO_EXCHANGE: 41,
  DAO_CONTRIBUTION: 42,
  DAO_CONFIRMATION: 43,

  // Coupon
  COUPON_ISSUER_AUDITOR_BUY: 49,
  COUPON_ISSUER_APPLY: 50,
  COUPON_ISSUER_CHECK: 51,
  COUPON_ISSUER_UPDATE: 52,
  COUPON_ISSUER_FREEZE: 53,
  COUPON_ISSUER_UNFREEZE: 54,
  COUPON_ISSUE_NEW: 55,
  COUPON_ISSUE_CLOSE: 56,
  COUPON_ISSUE_REOPEN: 57,
  COUPON_EXCH_BUY: 58,
  COUPON_EXCH_PAY: 59,
  COUPON_EXCH_TRANSFER_ASK: 71,
  COUPON_EXCH_TRANSFER_CONFIRM: 72,

  // AOB-ASSET ON BLOCKCHAIN: 60-79
  AOB_ISSUER: 60, // AOB ISSUER REGISTER
  AOB_ASSET: 61, // AOB ASSET REGISTER
  AOB_FLAG: 62, // AOB FLAGS UPDATE
  AOB_ACL: 63, // AOB ACL UPDATE
  AOB_ISSUE: 64, // AOB ISSUE
  AOB_TRANSFER: 65, // AOB TRANSFER

  LOCK: 100 // ACCOUNT LOCK
```
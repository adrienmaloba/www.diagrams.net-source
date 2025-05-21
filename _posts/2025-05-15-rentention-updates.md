---
layout: post
author: draw.io
slug: diagram-retention-confluence
date: 2025-05-16 09:54:00
title: Using draw.io with attachment retention rules in Confluence Data Center
tags: [features, Atlassian]
categories: [features,atlassian]
---

Retention rules in Confluence Data Center allow you to automatically delete historical versions of pages and attachments that you no longer need. draw.io diagrams are stored as page attachments. Therefore, the data retention settings you choose will apply to older versions of those diagrams. 

To implement a retention strategy, Confluence DC administrators need to set several rules.
* Apply global rules to all spaces in your Confluence instance, including archived and personal spaces. 
* Apply different rules for pages and for attachments. 
* Set exemptions and individual rules for spaces with longer data history requirements. 
* Set permissions that allow space administrators to set their own retention rules in their spaces. 
* Set a global rule or space exemptions for purging any manually deleted items that are in the trash. 

**Important:** Historical draw.io diagram versions, pages and other attachments that are deleted using these retention rules cannot be restored. Make sure your backup strategy takes this into account. 

Set the _coverage level_ to _Advanced_ or higher to ensure the [audit log](https://confluence.atlassian.com/doc/auditing-in-confluence-829076528.html) records all deletions and purges.

## Why use retention rules?

When [collaborating on a draw.io diagram in Confluence DC](/blog/collaborative-editing-confluence-dc.html), diagram attachment versions will be saved regularly to record everyone's contributions. If those diagrams include many embedded images, the size of those attachments can become quite large. Diagram versions will accumulate quickly during collaboration. 

Setting automatic deletion of old versions will [reduce the size of the Confluence database](https://confluence.atlassian.com/clean/clean-up-your-confluence-instance-1026047969.html) and attachment directory, and thus speed up backups and upgrades. 

**Note:** One of the main considerations for your data retention strategy is where teams are required to keep records of their work for compliance and auditing purposes.

## Which retention approach is best for diagrams? 

Retention rules apply to _all_ page attachments, not just attached diagrams. Choose rules that are appropriate for all attached content. 

**Important:** The order in which you set rules is important - when you set a global rule, it will be implemented immediately. 

Choose one of these retention strategies:

* Set the global rule to _keep all_ for both page and attachment versions, then set space exemptions to clean up specific spaces. 

* Add space exemptions to _keep all_ in spaces where you must retain the version history, then set a global rule to clean up all remaining non-critical spaces. This is useful when audits are required only on documentation in specific spaces. 

The default retention setting is to keep all pages and attachments and not purge the trash automatically.

If you find your instance is growing too large and slow, choose which versions of pages and attachments that you want to keep. 
*  keep by age
*  keep by version number, where the most recent ``x`` versions are kept
  
The second approach is likely more useful if you need to see how a diagram was developed and by whom.

Refer to [Atlassian's documentation to see how to set retention rules](https://confluence.atlassian.com/doc/set-retention-rules-to-delete-unwanted-data-1108681072.html) as an administrator. 

The latest versions are never deleted even if that version is older than the retention rule - only the historical versions are deleted. 

**When are old versions deleted?**

A [scheduled job](https://confluence.atlassian.com/doc/scheduled-jobs-96567525.html) will run every 10 minutes to permanently delete a small batch of outdated versions so as not to overwhelm your instance. 

As an administrator, you can manually run the 'hard' job which will delete all outdated versions. Only do this when your instance is not busy. 



## Migrating to Cloud - set retention rules before migration

Purge older versions of pages and attachments _before you start migrating_ so there will be much less data that needs to be copied and ensure your migration happens more quickly. 

[See how to update pageIDs to migrate with draw.io from Confluence DC to Cloud](https://www.drawio.com/doc/faq/migrate-drawio-confluence)


# Microblog Recommendation Datasets
## Introduction
The datasets contain Sina Weibo dataset and Twitter dataset. 
The Sina Weibo dataset are collected from Sina Weibo (weibo.com), containing 2,792 users with 216,176 microblogs.
The Twitter dataset are collected from Twitter (twitter.com), including 1,267 users with 265,033 microblogs.
Both datasets contain four kinds of documents:
* user_uid.dat: the microblogs of user uid, each line is a microblog.
* user_uid_follow.dat: the microblogs of user uid's all followed users, and each line is a microblog.
* user_uid_followed_user.dat: a list, the followed user set of user uid.
* user_uid_social.dat: a dictionary, the followed user set of all users (including user uid and uid's followed users).

### microblog structure:
microblog {
	"id": microblog id,
	"userid": the user id of the microblog author,
	"time": the time that the microblog is posted,
	"text": microblog text content,
	"attitudes_count": number of like,
	"comments_count": number of comments,
	"reposts_count": number of repost.
	"has_link": whether the microblog contains video links,
	"has_pic": whether the microblog contains pictures,
	"topic": a list, contains topics in the microblog,
	"original": if this is a re-posted microblog, it contains the original microblog. 
}

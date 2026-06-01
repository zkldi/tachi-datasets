## In short: These are large rhythm game score datasets, free to use.

# Tachi Datasets

[Tachi](https://github.com/zkldi/Tachi) is a rhythm game website that tracks your scores on all your favourite games, and provides _awesome_ features like quests, sessions, rivals, and more!

We think it'd be in people's interest to have open, easy-to-use access to the millions of scores and sessions we have on Tachi.

There's no shortage of cool stuff you can do with this data - you could run stats to find out what charts people struggle on, how certain charts have gotten more or less popular over the years...

In short, **you're free to do whatever you want with these large rhythm game datasets**.

I hope it helps you out! I sure wish I had something this practical when I was starting out.

# Recommended Usage

If you are developing stuff for Tachi and need some local data to play with, this is invaluable. **Note that you can log into any users account with `password` as the password!**

If you are a stats nerd, or just a rhythm game nerd in general, this is an excellent resource for doing any sort of analysis. Have fun!

# Usage from Local Tachi

If you have [Tachi](https://github.com/zkrising/Tachi) set up on your local machine, you can use `just load-kamai-dataset` or `just load-boku-dataset`.

# Usage

Download the dump you want from the CDN.

## Kamaitachi

- https://cdn.tachi.ac/datasets/tachi-kamai-2026-06.sql.gz

## Bokutachi

- https://cdn.tachi.ac/datasets/tachi-boku-2026-06.sql.gz

Run `gunzip -c "$filename" | psql -d "$db_url"` to restore the database. If you don't understand what this means, go to the [Tachi Repo](https://github.com/zkldi/Tachi), get set up, and run `just db-load-dataset`.

## Anonymisation

This dataset has been anonymised to the best of our ability; no usernames or about me's or anything like that is present.

**All passwords are set to `password`.**

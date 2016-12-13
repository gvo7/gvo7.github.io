---
layout: post
title:  "Posting about Elexir and the Phoenix Framework"
date:   2016-12-13 18:00:01 +0200
categories: elexir phoenix
---

Test code snippets of Elexir

{% highlight vim %}
mix phoenix.new hello
{% endhighlight %}


{% highlight elixir %}
defmodule Productlayer.Repo.Migrations.CreateUser do
  use Ecto.Migration

  def change do
    create table(:users) do
      add :name, :string
      add :username, :string, null: false
      add :password_hash, :string
      add :mail, :string

      timestamps()
    end

    create unique_index(:users, [:username])
  end
end
{% endhighlight %}

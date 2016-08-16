---
layout: post
title: "Rails Validates"

---

```
class Product < ActiveRecord::Base
  validates :title, :description, :image_url, :presence => true
end
```

validates
方法是标准的Rails验证器，它根据一个或者多个条件来验证一个或者多个模型字段

```
  validates :title, :description, :image_url, :presence => true
```

- :presence => true
- :numericality => {:greater_than_or_equal_to => 0.01}
- :uniqueness => true
- :format => {
             :with => %r{\.(gif|jpg|png)$}i,
			 :message => 'must be a URL for GIF, JPG or PNG image.'
			 }


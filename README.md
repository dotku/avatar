# avatar

Compared over 15 avatar image provider, and create a service for the community.

## Usage

```jsx
import { Avatar } from "@nextui-org/react";
import { useAppAvatar } from "@/hooks/useAppAvatar";

export default function AppAvatar({user}) {
  const {avatarURL, loading} = useAppAvatar({user});

  return loading ? <Avatar name={user.firstName} /> : <Avatar
      src={avatarURL}
      name={user.firstName}
    />;
}
```

## Ideas

could use this input to identify the avatar

```
{
  user = {email: "name@domain.tld", name: "first_name last_name"}
  provider = "dicebear"
  style = "adventurer",
  format = "svg",
}
```

## Reference

1. gravatar

    Usually it would be usued for someone already existed on the social platform, 
    which might be helpful for general social purpose, but not great for a product
    that focusing on the social or other senstive content, eg finance.

2. pravatar.cc

    It has limit on number you can query everyday :(

3. ui-avatars

    It is simple but... not sure if name is that much usually, it is great for 
    fallback image placeholder.

4. josechmoe [under maintain]

    It was under maintain when I was checking... no comment on it.

5. dicebear

    It is down :(

6. robohash

    A robot theme?! Interesting

7. placeholder [aquired]

    Aquired by other company?!

8. baconmockup

    It looks gross :(

9. fillmurray [down]

    it is down :(

10. placekitten [down]

    It is down...

11. placebear

    How can it be random image?

12. placecage [down]

    a service that can be used to fetch pictures of Nicolas Cage

13. placebeard.it

    Gender equality?

14. placedog

    Down

15. dicebear

    Provides serveral different styles for user to pickup,
    I think dicebear so far would be the best avatar service that provides fast and rich styles for your social project need

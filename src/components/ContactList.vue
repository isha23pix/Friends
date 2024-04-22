<template>
  <v-container fluid>
    <v-list>
      <v-card
        @click="openChat(chat)"
        v-for="chat in chats"
        :key="chat.id"
        two-line
      >
        <v-card-actions>
          <v-row no-gutters align="center">
            <!-- Avatar Column -->
            <v-col cols="2">
              <v-avatar>
                <img :src="chat.friend_photo" alt="Profile image" />
              </v-avatar>
            </v-col>

            <!-- Name and Message Column -->
            <v-col cols="4">
              <v-list-item-content>
                <v-list-item-title>{{ chat.friend_name }}</v-list-item-title>
                <v-list-item-subtitle>{{
                  chat.last_message
                }}</v-list-item-subtitle>
              </v-list-item-content>
            </v-col>

            <!-- Seen/Unseen Icon and Time -->
            <v-col cols="4">
              <v-row justify="end">
                <div class="justify-self-end">
                  <v-list-item-action class="me-1">
                    <div v-if="chat.unread_message_count > 0">
                      <v-badge
                        color="#6e00ff"
                        :content="chat.unread_message_count"
                      >
                        <v-icon color="grey">mdi-message</v-icon>
                      </v-badge>
                    </div>
                    <div v-else>
                    <!-- <v-icon :color="chat.seen ? '6e00ff' : 'default'">
                      {{ chat.seen ? 'mdi-check-all' : 'mdi-check' }}
                    </v-icon> -->
                  </div>
                  </v-list-item-action>
                  <!-- <v-list-item-action-text class="custom-time">{{ chat.time }}</v-list-item-action-text> -->
                </div>
              </v-row>
            </v-col>
          </v-row>
        </v-card-actions>
      </v-card>
    </v-list>
  </v-container>
</template>

<script>
import axios from "axios";
export default {
  name: "ChatList",
  data() {
    return {
      chats: [],
    };
  },
  methods: {
    openChat(chat) {
      // Here you can emit an event or directly call a method in the parent component
      // to update the profile icon and name in the ChatBox component
      console.log("Selected chat:", chat);
      this.$emit("update-chat-box", chat);
    },
    async getAllConversationsData() {
      await axios
        .get(`http://localhost:3000/api/friends/getMyAllConversations/2`)
        .then((response) => {
          console.log(response.data);
          this.chats = response.data;
        })
        .catch((error) => {
          console.error("Error fetching user groups:", error);
        });
    },
  },
  mounted() {
    this.getAllConversationsData();
  },
};
</script>

<style scoped>
.v-container {
  border-radius: 5px;
}
.v-list-item {
  margin-bottom: 8px;
}

::v-deep .v-avatar img {
  border-radius: 50%; /* Makes the image round */
  width: 40px; /* Controls the width of the image */
  height: 40px; /* Controls the height of the image */
}

.v-list-item-action-text {
  margin-right: 10px;
}

.v-card {
  background-color: #ffffff;
  padding-top: 8px;
}

.v-list-item {
  align-items: center; /* Ensures vertical alignment is centered */
}

.custom-time {
  color: #555; /* Change the color of the time text */
}
</style>

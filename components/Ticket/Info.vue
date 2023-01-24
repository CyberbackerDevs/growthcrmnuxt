<template>
    <div class="d-ticket-info">
        <div class="d-ticekt-left">
            <div class="d-ticekt-title">Sample ticket info</div>
            <div class="d-stats-prio">Sent by <span class="ds-name">Jonhn Peter Doe</span> on <span class="ds-date">November 5, 2022</span></div>
            <div class="d-ticket-detailed-info">
                <div class="d-info-part">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In id ex ac mauris condimentum imperdiet a sit amet tellus. Nullam in lorem vel lorem viverra luctus. Vestibulum nec sapien elit. Curabitur vel lectus dictum, efficitur nisi sed, vehicula urna. Etiam aliquam dignissim iaculis. Pellentesque magna felis, laoreet id sollicitudin ac, varius eget nulla. Cras tincidunt et lectus vel congue. Vivamus ac orci a turpis luctus imperdiet eu et velit. Duis quis risus sem. Sed et dolor vitae tortor luctus consequat. Duis vel varius nisi, eget fringilla augue.</p>
                    <p>Suspendisse eget sapien ut metus volutpat aliquet a eu mi. Maecenas pharetra ligula mi, ac accumsan ante ultricies et. Phasellus non facilisis nisi, vel porttitor sem. Maecenas ornare quis magna at auctor. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Phasellus lacinia, risus vel accumsan feugiat, ipsum velit viverra turpis, ac aliquet arcu tellus quis erat. Nunc vulputate finibus diam, eget fringilla nibh fermentum at. Pellentesque semper velit ac est vestibulum, ac pretium felis tincidunt. Fusce est lacus, viverra at commodo ac, tincidunt id eros. Vestibulum in quam sed mauris lacinia porta in ut velit. Cras sed lectus venenatis, semper erat eget, elementum dui. Pellentesque ac dolor scelerisque, rutrum diam vitae, fermentum purus.</p>
                    <p>Fusce eu nisi sed nulla luctus pharetra. In sed leo est. Ut in tortor ipsum. Mauris id scelerisque metus. Sed eleifend malesuada ligula, nec semper enim consequat sit amet. Pellentesque vestibulum gravida turpis, non semper nunc commodo quis. Curabitur accumsan consectetur elementum. In at lacus odio.</p>
                </div>
            </div>
            <div class="comment_section">
                <div class="comment-header-title">Comments</div>
                <div class="comment_add_one">
                    <tiptap-vuetify class="add-comment" :toolbar-attributes="{ color: 'yellow' }" v-model="content" :extensions="extensions"/>
                </div>
                <div class="adding-comment-options">
                    <button class="d-add-save-button">Save</button>
                </div>
                <div class="comments_list">
                    <div class="comment_item" v-for="(item, index) in comments" :key="index">
                        <div class="d-comment-item-inner">
                            <div class="d-comment-name">{{item.name}}</div>
                            <div class="d-comment-date">{{item.date}}</div>
                            <div class="d-comment-info">{{item.message}}</div>
                        </div>
                    </div>
                </div>
            </div>
        </div> 
        <div class="d-ticket-right">
            <div class="stats-list">
                <div class="d-stats-item">
                    <div class="d-stats-title">Tags</div>
                    <div class="d-stats-details">
                        <v-combobox
                        multiple
                        small-chips
                        solo
                        ></v-combobox>
                    </div>
                </div>
                <div class="d-stats-item">
                    <div class="d-stats-title">Assignee</div>
                    <div class="d-stats-details">
                        <v-combobox
                        multiple
                        small-chips
                        solo
                        ></v-combobox>
                    </div>
                </div>
                <div class="d-stats-item">
                    <div class="d-stats-title">Priority</div>
                    <div class="d-stats-details">
                        <v-select
                            :items="priority"
                            label="Standard"
                            solo
                        ></v-select>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import {
        TiptapVuetify,
        Heading,
        Bold,
        Italic,
        Strike,
        Underline,
        Code,
        Paragraph,
        BulletList,
        OrderedList,
        ListItem,
        Link,
        Blockquote,
        HardBreak,
        HorizontalRule,
        History
    } from 'tiptap-vuetify'

    export default {
        name: 'CPayslip',
        components: { TiptapVuetify },
        data () {
            return {
                dialog: false,
                priority: ['Foo', 'Bar', 'Fizz', 'Buzz'],
                comments: [
                    {
                        id: 123,
                        name: 'some cb',
                        user_id: 3452134,
                        message: 'Fusce eu nisi sed nulla luctus pharetra. In sed leo est. Ut in tortor ipsum. Mauris id scelerisque metus. Sed eleifend malesuada ligula, nec semper enim consequat sit amet. Pellentesque vestibulum gravida turpis, non semper nunc commodo quis. Curabitur accumsan consectetur elementum. In at lacus odio.',
                        date: 'Nov. 12, 2022',
                        order: 1,
                    },
                    {
                        id: 123,
                        name: 'some cb',
                        user_id: 3452134,
                        message: 'Fusce eu nisi sed nulla luctus pharetra. In sed leo est. Ut in tortor ipsum. Mauris id scelerisque metus. Sed eleifend malesuada ligula, nec semper enim consequat sit amet. Pellentesque vestibulum gravida turpis, non semper nunc commodo quis. Curabitur accumsan consectetur elementum. In at lacus odio.',
                        date: 'Nov. 12, 2022',
                        order: 1,
                    },
                    {
                        id: 123,
                        name: 'some cb',
                        user_id: 3452134,
                        message: 'Fusce eu nisi sed nulla luctus pharetra. In sed leo est. Ut in tortor ipsum. Mauris id scelerisque metus. Sed eleifend malesuada ligula, nec semper enim consequat sit amet. Pellentesque vestibulum gravida turpis, non semper nunc commodo quis. Curabitur accumsan consectetur elementum. In at lacus odio.',
                        date: 'Nov. 12, 2022',
                        order: 1,
                    },
                    {
                        id: 123,
                        name: 'some cb',
                        user_id: 3452134,
                        message: 'Fusce eu nisi sed nulla luctus pharetra. In sed leo est. Ut in tortor ipsum. Mauris id scelerisque metus. Sed eleifend malesuada ligula, nec semper enim consequat sit amet. Pellentesque vestibulum gravida turpis, non semper nunc commodo quis. Curabitur accumsan consectetur elementum. In at lacus odio.',
                        date: 'Nov. 12, 2022',
                        order: 1,
                    },
                    {
                        id: 123,
                        name: 'some cb',
                        user_id: 3452134,
                        message: 'Fusce eu nisi sed nulla luctus pharetra. In sed leo est. Ut in tortor ipsum. Mauris id scelerisque metus. Sed eleifend malesuada ligula, nec semper enim consequat sit amet. Pellentesque vestibulum gravida turpis, non semper nunc commodo quis. Curabitur accumsan consectetur elementum. In at lacus odio.',
                        date: 'Nov. 12, 2022',
                        order: 1,
                    },
                    {
                        id: 123,
                        name: 'some cb',
                        user_id: 3452134,
                        message: 'Fusce eu nisi sed nulla luctus pharetra. In sed leo est. Ut in tortor ipsum. Mauris id scelerisque metus. Sed eleifend malesuada ligula, nec semper enim consequat sit amet. Pellentesque vestibulum gravida turpis, non semper nunc commodo quis. Curabitur accumsan consectetur elementum. In at lacus odio.',
                        date: 'Nov. 12, 2022',
                        order: 1,
                    },
                    {
                        id: 123,
                        name: 'some cb',
                        user_id: 3452134,
                        message: 'Fusce eu nisi sed nulla luctus pharetra. In sed leo est. Ut in tortor ipsum. Mauris id scelerisque metus. Sed eleifend malesuada ligula, nec semper enim consequat sit amet. Pellentesque vestibulum gravida turpis, non semper nunc commodo quis. Curabitur accumsan consectetur elementum. In at lacus odio.',
                        date: 'Nov. 12, 2022',
                        order: 1,
                    },
                ],
                content: '<p></p><p></p><p></p>',
                extensions: [
                    History,
                    Blockquote,
                    Link,
                    Underline,
                    Strike,
                    Italic,
                    ListItem,
                    BulletList,
                    OrderedList,
                    [
                        Heading,
                        {
                        options: {
                            levels: [1, 2, 3]
                        }
                        }
                    ],
                    Bold,
                    Link,
                    Code,
                    HorizontalRule,
                    Paragraph,
                    HardBreak
                ],
                    // starting editor's content
                    
            }
        },
        methods: {
            openSpecificPayslip(){
                this.dialog = true;
            }
        }
    }
</script>

<style scoped>
    .d-ticket-info .d-ticekt-left {
        display: inline-block;
        width: 70%;
        vertical-align: top;
    }

    .d-ticket-info .d-ticket-right {
        display: inline-block;
        width: 28%;
        vertical-align: top;
    }

    .d-ticekt-title {
        font-size: 21px;
        line-height: 1.2em;
    }

    .d-stats-prio {
        margin-bottom: 15px;
        font-size: 14px;
    }

    .d-info-part p {
        margin-bottom: 15px;
        text-align: justify;
    }

    .d-comment-name {
        font-size: 16px;
        font-weight: bold;
    }

    .d-comment-date {
        font-size: 13px;
        color: #333;
        margin-bottom: 20px;
    }

    .comment_item {
        border-bottom: 1px solid #ccc;
        padding: 20px;
    }

    .comment-header-title {
        font-weight: 400;
        font-size: 18px;
        border-bottom: 1px solid #ccc;
        padding-bottom: 5px;
        margin-bottom: 15px;
    }

    .d-ticket-detailed-info {
        margin-bottom: 50px;
    }

    .adding-comment-options {
        text-align: right;
    }
    
    button.d-add-save-button {
        background: #333333;
        color: #fff;
        font-size: 14px;
        text-transform: uppercase;
        line-height: 1em;
        padding: 10px 20px;
        border-radius: 5px;
    }

    .comment_add_one {
        margin-bottom: 10px;
    }

    .stats-list {
        padding-left: 25px;
        margin-top: 60px;
    }

    .stats-list .d-stats-item {
        margin-bottom: 20px;
    }

    .stats-list .d-stats-item .d-stats-title {
        font-size: 16px;
        font-weight: bold;
        margin-bottom: 5px;
    }

    
    

</style>

<style>
    .tiptap-vuetify-editor.add-comment header.v-sheet {
        background: #333;
        color: #fff !important;
    }

    .tiptap-vuetify-editor.add-comment header.v-sheet .theme--light.v-btn.v-btn--icon {
        color: #fff;
    }

    .tiptap-vuetify-editor.add-comment .tiptap-vuetify-editor__content p {
        min-height: 1rem;
    }
</style>